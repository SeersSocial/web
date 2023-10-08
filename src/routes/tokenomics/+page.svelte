<script>
	import chart from "$lib/images/chart.png"
	import allocation from "$lib/images/allocation.png"
</script>
<svelte:head>
	<title>Token</title>
	<meta name="description" content="Token Economics" />
</svelte:head>

<section class="w-full flex flex-col mt-14 text-lg justify-center justify-items-center content-center items-center">

	<div class="flex flex-col md:w-2/3 gap-4">
		<h2 class="font-bold text-emerald-500">Tokenomics Overview</h2>
		<p class="">The heart of ICX tokenomics revolves around a clear cap on the total supply, ensuring the total number of ICX tokens will never surpass 150 million. As of the current state, the supply stands at 100 million ICX tokens. The distribution of these tokens is delineated as follows:</p>
		<ul class="list-inside space-y-4">
			<li><span class="underline decoration-emerald-400">Dev Team:</span> 15% of the total supply, equating to 15 million ICX tokens, is reserved for the development team. These tokens are vested over a span of 4 years, underscoring the team's long-term dedication to the project and synchronizing their interests with the continued evolution and success of the platform.</li>
			<li><span class="underline decoration-emerald-400">Community:</span> 17% of the tokens, amounting to 17 million ICX tokens, are held by the broader community. This allocation is devised to amplify active participation and nurture a deep-rooted sense of ownership and collaborative decision-making within the ecosystem.</li>
			<li><span class="underline decoration-emerald-400">Treasury:</span> The rest of the tokens, after deducing the allocations for the dev team and community, is safeguarded in the treasury. The primary purpose of the treasury is to fortify the project's long-term resilience, facilitating future developmental strides, forging partnerships, and spearheading other essential initiatives.</li>
		</ul>
        <img src={allocation} alt="" class="rounded" />
		<h2 class="font-bold text-purple-500 mt-2">Inflationary Trajectory</h2>
		<p>
			The ICX token model takes shape around a meticulously devised inflationary curve, inaugurating with an inflation rate of 10%. This rate is designed to gracefully taper, converging towards 0% over a clear-cut 12-year duration.
		</p>
        <h3 class="font-bold mt-2">Comparison with Bitcoin's Monetary Policy</h3>
		<p class="mb-4 font-medium">
			While Bitcoin has established its legacy in the cryptocurrency realm with its deflationary issuance model marked by periodic halvings, ICX offers a unique paradigm. It champions a uniform and measured reduction in inflation, crafting a predictable course over its 12-year timeline.
		</p>
        <img src={chart} alt="" class="rounded" />
		<h2 class="font-bold text-sky-500">Advantages</h2>
        <ul class="list-inside space-y-4">
			<li><span class="underline decoration-sky-400">Incentivized Engagement:</span> The tokenomics fosters network participation, with the initial inflation rate tailored to boost active engagement and community growth.</li>
			<li><span class="underline decoration-sky-400">Balanced Economic Model:</span> The ICX model strives for consistent growth, avoiding drastic changes that might lead to market volatility.</li>
			<li><span class="underline decoration-sky-400">Stakeholder Alignment:</span> By having a clear token allocation strategy, ICX ensures vested interest among developers, community members, and strategic planners in the project's success.</li>
            <li><span class="underline decoration-sky-400">Future-Proofed Treasury:</span> The treasury's significant token allocation ensures a robust reserve for pivots, expansions, or unforeseen challenges, securing the network's future.</li>
        </ul>
        <h2 class="font-bold text-pink-500">Conclusion</h2>
        <p class="mb-4 font-medium">
            ICX's tokenomics is a meticulous fusion of strategic planning and community-driven priorities. It's designed to offer both immediate incentives for participation and the foundation for long-term network sustainability. Importantly, the ICX token serves as a utility within its ecosystem, and its distribution or use should not be viewed as a speculative instrument or a security.
        </p>
    </div>
</section>
