<script>
    import { Accordion, AccordionItem } from "flowbite-svelte";
    import Groq from 'groq-sdk';
	import { onMount } from "svelte";

    const groqKey = "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"

    const main = async ()  => {
        const groq = new Groq();

        const chatCompletion = await groq.chat.completions.create({
            messages: [{ role: 'user', content: 'Explain the importance of low latency LLMs' }],
            model: 'mixtral-8x7b-32768',
        });

        console.log(chatCompletion.choices[0].message.content);
    }

    onMount(main)
</script>

<svelte:head>
	<title>AI</title>
	<meta name="description" content="AI" />
</svelte:head>
