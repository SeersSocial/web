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
    let personalities = [
        "Emma, Retail Manager. Biography: Emma, 32, manages a bustling boutique in the city center. She has a degree in Business Administration and has worked her way up from sales assistant to manager over the past ten years. Personality: Emma is energetic and personable, with a knack for understanding customer needs and trends. She's decisive and highly organized, often handling multiple challenges simultaneously with a calm demeanor.",
        "Dr. John, Cardiologist.  Biography: Dr. John, 45, is a cardiologist at a prominent hospital. After completing his medical degree and a demanding residency, he now leads a team of healthcare professionals. Personality: Dr. John is meticulous and compassionate, always taking the time to explain procedures and care plans to his patients. His colleagues respect him for his leadership skills and his dedication to patient care.",
        "Luis,  Industrial Engineer. Biography: Luis, 38, works in a large manufacturing plant where he designs efficient systems to improve production lines. He holds an engineering degree and has a keen interest in automation. Personality: Analytical and detail-oriented, Luis is always looking for ways to optimize processes. He is patient and methodical, making him excellent at solving complex problems.",
        "Sophia, Elementary School Teacher. Biography: Sophia, 28, teaches first grade in a vibrant community school. She has a passion for early childhood education and holds a Master's degree in the field. Personality: Warm and creative, Sophia has a natural talent for making learning fun and accessible. She is patient and caring, creating a supportive and nurturing classroom environment.",
        "Isabel, Construction Project Manager. Biography: Isabel, 40, leads large construction projects, ensuring they are completed on time and within budget. She has a degree in civil engineering and a wealth of experience in the construction industry. Personality: Strong-willed and highly competent, Isabel thrives in high-pressure environments. She is both a team leader and a team player, respected for her strategic thinking and problem-solving abilities.",
        "Mike,  Delivery Driver. Biography: Mike, 30, works for a national logistics company, ensuring timely delivery of goods across the region. He has extensive experience in transportation and logistics management. Personality: Dependable and hardworking, Mike takes pride in his job and is always looking to improve his routes and delivery times. He's friendly and enjoys the daily interactions with clients on his routes.",
        "Rachel, Social Worker. Biography: Rachel, 34, is a social worker who assists families in navigating various challenges. She has a degree in social work and specializes in child welfare. Personality: Empathetic and resilient, Rachel is driven by a strong desire to help others. She's an excellent listener and advocate, known for her ability to connect with and support her clients in meaningful ways."
    ]
    let names = ["Emma", "Dr. John", "Luis", "Sophia", "Isabel", "Mike", "Rachel"]

    const main = async ()  => {
        if (!content) return

        for (let i = 0; i < personalities.length; i++) {
            let messages_tmp = []
            for (let j = Math.max(responses.length - names.length, 0); j < responses.length; j++) {
                messages_tmp.push({ role: 'user', content: names[j % names.length] + ": " + responses[j] })
            }
            
            let messages = messages_tmp.slice()
            let prompt = [{ role: 'user', content: "Generate a unique short response that is coherent with the dialogue history, without repeating previous sentences. Use methaphors." }, { role: 'user', content }];
            messages = messages.concat(prompt)

            const chatCompletion = await groq.chat.completions.create({
                messages,
                model: 'llama3-70b-8192',
            });

            response = chatCompletion.choices[0].message.content;
            responses.push(response) 
            responses = responses   
        }

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
        <Button type="submit" on:click={main} color="dark" class="border-none outline-none hover:outline-none focus:outline-none shadow-none ring-black ring-0 focus:ring-0">Post</Button>
    </div>
    <div class="grid grid-cols-4 gap-4 w-full m-2 p-2">
        {#each responses as r, i}
            <div class="w-full bg-white text-black rounded-lg p-2"><span class="font-bold mr-1">{names[i % names.length]}</span> {r}</div>
        {/each}
    </div>
</div>