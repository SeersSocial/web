<script>
    import { Input, Button } from "flowbite-svelte";
    import Groq from 'groq-sdk';
	import { onMount } from "svelte";

    const groqKey = "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"
    const groq = new Groq({
        apiKey: groqKey,
        dangerouslyAllowBrowser: true
    });

    let content = ""
    let response = ""

    const main = async ()  => {
        console.log("calling groq")

        const chatCompletion = await groq.chat.completions.create({
            messages: [{ role: 'user', content }],
            model: 'mixtral-8x7b-32768',
        });

        response = chatCompletion.choices[0].message.content;
    }

    onMount(main)
</script>

<svelte:head>
	<title>AI</title>
	<meta name="description" content="AI" />
</svelte:head>

<div class="w-full">
    <Input type="text" id="post" placeholder="Post something" bind:value={content}/>
    <Button type="submit" on:click={main}>Submit</Button>
</div>
<div class="w-full">
    {response}
</div>