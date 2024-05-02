<script>
// @ts-nocheck

    import { Input, Button, Card } from "flowbite-svelte";
    import Groq from 'groq-sdk';
	
    const groq = new Groq({
        apiKey: import.meta.env.VITE_GROQ_API_KEY,
        dangerouslyAllowBrowser: true,
    });

    let content = ""
    let response = ""
    let responses = []

    const main = async ()  => {
        if (!content) return

        const chatCompletion = await groq.chat.completions.create({
            messages: [ 
                { role: 'user', content: "Reply with less than 300 characters. Reply with personality as a human replying to a post. Don't use hashtags or anything that can imply you are a bot. Remove quotes. Reply to the following:" }, 
                { role: 'user', content }
            ],
            model: 'llama3-70b-8192',
        });

        response = chatCompletion.choices[0].message.content;
        responses.push(response)
        responses = responses
        content = ""
    }

</script>

<svelte:head>
	<title>AI</title>
	<meta name="description" content="AI" />
</svelte:head>

<div class="w-full p-2 m-2 gap-4 min-h-screen">
    <div class="flex flex-row w-full m-2 p-2 gap-2">
        <Input type="text" id="post" placeholder="Write something" bind:value={content}/>
        <Button type="submit" on:click={main} color="dark" class="border-none outline-none hover:outline-none focus:outline-none shadow-none ring-black ring-0">Post</Button>
    </div>
    <div class="grid grid-cols-4 gap-4 w-full m-2 p-2">
        {#each responses as r}
            <div class="w-full bg-white text-black rounded-lg p-2">{r}</div>
        {/each}
    </div>
</div>