<script>
	import network from "$lib/images/network.jpeg"
	import revolution from "$lib/images/revolution.jpeg"
</script>
<svelte:head>
	<title>About</title>
	<meta name="description" content="About ICX" />
</svelte:head>

<section class="w-full flex flex-col mt-14 text-lg justify-center justify-items-center content-center items-center">

	<div class="flex flex-col md:w-2/3 gap-4">
		<h2 class="font-bold text-sky-500">What is ICX?</h2>
		<p class="">ICX is a cutting-edge web3 social network designed to embody the true principles of a decentralized internet. Built atop the revolutionary framework of the Internet Computer, it mirrors the functionalities you love on platforms like Twitter, but with enhanced privacy, ownership, and community-driven governance.</p>
		<img src={network} alt="" class="rounded h-200" />
		<h2 class="font-bold text-emerald-500 mt-2">Key Features</h2>
		<ul class="list-inside space-y-4">
			<li><span class="underline decoration-emerald-400">True Ownership:</span> On ICX, your content is yours. Leveraging the principles of web3, users have true ownership of their posts, images, and videos. This means you can benefit directly from the value your content generates, without intermediaries taking a disproportionate cut.</li>
			<li><span class="underline decoration-emerald-400">Community Governance:</span> ICX is not just a platform; it's a community. Decisions about the network's rules, algorithms, and future developments are made collectively by its users. Your voice genuinely matters here.</li>
			<li><span class="underline decoration-emerald-400">Enhanced Privacy:</span> Say goodbye to invasive ads and data mining. ICX values your privacy. With end-to-end encryption and VetKeys protocols, your personal information and conversations remain confidential.</li>
			<li><span class="underline decoration-emerald-400">Token-Based Economy:</span> ICX integrates a native token system, allowing users to earn, spend, or trade tokens based on their activity and contributions to the platform. Whether you're a content creator or an active participant in discussions, there's an opportunity to earn.</li>
			<li><span class="underline decoration-emerald-400">Interoperability:</span> Being built on the Internet Computer, ICX offers seamless integration with other decentralized apps and platforms. This ensures that as the web3 ecosystem grows, ICX users will be at the forefront of innovation and connectivity.</li>
			<li><span class="underline decoration-emerald-400">Resilient & Censorship-Resistant:</span> Thanks to its decentralized infrastructure, ICX is highly resistant to attacks, censorship, and centralized control. No matter where you are in the world, your voice can be heard without fear of suppression.</li>
		</ul>
		<h2 class="font-bold text-purple-500 mt-2">Harnessing AI for an Elevated Experience</h2>
		<p>
			Incorporating the latest in artificial intelligence, ICX transcends traditional social networking capabilities. Our AI-enhanced features streamline content discovery, tailoring your feed to resonate with your preferences while minimizing echo chambers. AI also powers our advanced content moderation, ensuring a safe and positive environment for all users. Additionally, our smart analytics provide insights for content creators, helping them understand their audience and optimize engagement. With AI at its core, ICX not only redefines social interactions but also augments user experience to new heights.
		</p>
		<img src={revolution} alt="" class="rounded h-200" />
		<h2 class="font-bold text-pink-500 mt-2">Join the Revolution</h2>
		<p class="mb-4 font-medium">
			The internet is evolving, and ICX is at the forefront of this change. Join us in shaping the future of social networking, where power returns to the people, and creativity thrives unbounded.
		</p>
	</div>
</section>
