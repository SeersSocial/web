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
                { role: 'user', content: "Generate a response that is coherent with the dialogue history. Desired traits for responses are: 1) Relevant - The response addresses the context, 2) Informative - The response provides some information, 3) Interesting - The response is not interesting, 4) Consistent - The response is consistent with the rest of the conversation in terms of tone and topic, 5) Helpful - The response is helpful in providing any information or suggesting any actions, 6) Engaging - The response is not very engaging and does not encourage further conversation, 7) Specific - The response contains pecific content, 9) User understanding - The response demonstrates an understanding of the user's input and state of mind, and 10) Fluent. Response should be less than 300 characters." }, 
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