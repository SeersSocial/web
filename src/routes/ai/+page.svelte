<script>
// @ts-nocheck

    import { Input, Button, Card } from "flowbite-svelte";
    import Groq from 'groq-sdk';
	import { onMount } from "svelte";

    const groqKey = "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"
    const groq = new Groq({
        apiKey: groqKey,
        dangerouslyAllowBrowser: true
    });

    let content = ""
    let response = ""
    let responses = []

    const main = async ()  => {
        console.log("calling groq")
        if (!content) return

        const chatCompletion = await groq.chat.completions.create({
            messages: [{ role: 'user', content }],
            model: 'mixtral-8x7b-32768',
        });

        response = chatCompletion.choices[0].message.content;
        responses.push(response)
    }

    onMount(main)
</script>

<svelte:head>
	<title>AI</title>
	<meta name="description" content="AI" />
</svelte:head>

<div class="w-full p-2 m-2 gap-4 min-h-screen">
    <div class="w-[300px] m-2 p-2">
        <Input type="text" id="post" placeholder="Write something" bind:value={content}/>
        <Button type="submit" on:click={main} color="dark" class="focus:outline-none">Post</Button>
    </div>
    <div class="w-full m-2 p-2 gap-1">
        {#each responses as r}
            <Card>{r}</Card>
        {/each}
    </div>
</div>