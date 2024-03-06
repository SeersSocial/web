<script>
	import chart from "$lib/images/chart.png"
	import allocation from "$lib/images/allocation.png"
</script>
<svelte:head>
	<title>Token</title>
	<meta name="description" content="Token Economics" />
</svelte:head>

<section class="w-full flex flex-col text-lg justify-center justify-items-center content-center items-center">

	<div class="flex flex-col md:w-2/3 gap-4">
		<h2 class="font-bold text-emerald-500">Tokenomics Overview</h2>
		<p class="">The heart of ICX tokenomics revolves around avoiding inflation by keeping a fixed supply of 100 million ICX tokens. The distribution of these tokens is delineated as follows:</p>
		<ul class="list-inside space-y-4">
			<li><span class="underline decoration-emerald-400">Dev Team:</span> 15% of the total supply, equating to 15 million ICX tokens, is reserved for the development team. These tokens are vested over a span of 4 years, underscoring the team's long-term dedication to the project and synchronizing their interests with the continued evolution and success of the platform.</li>
			<li><span class="underline decoration-emerald-400">Community:</span> 17% of the tokens, amounting to 17 million ICX tokens, are held by the broader community. This allocation is devised to amplify active participation and nurture a deep-rooted sense of ownership and collaborative decision-making within the ecosystem.</li>
			<li><span class="underline decoration-emerald-400">Treasury:</span> The rest of the tokens, after deducing the allocations for the dev team and community, is safeguarded in the treasury. The primary purpose of the treasury is to fortify the project's long-term resilience, facilitating future developmental strides, forging partnerships, and spearheading other essential initiatives.</li>
		</ul>
        <img src={allocation} alt="" class="rounded" />
    </div>
</section>
