<script>
	import { A } from "flowbite-svelte";

	import { Principal } from "@dfinity/principal";
	import { defaultAgent, uint8ArrayToHexString } from "@dfinity/utils";
	import { initSnsWrapper, neuronSubaccount } from "@dfinity/sns";
	import { onMount } from "svelte";

	const readGovernance = async () => {
		console.log("executing read governance")
		const agent = defaultAgent();
		const snsWrapper = await initSnsWrapper({
			rootOptions: {
				canisterId: Principal.fromText("u67kc-jyaaa-aaaaq-aabpq-cai"),
			},
			agent,
			certified: false,
		});

		let beforeNeuronId = undefined
		let neurons = []
		let totalStake = BigInt(0)
		let totalNeurons = BigInt(0)
		let totalMaturity = BigInt(0)
		let totalMaturityDevs = BigInt(0)

		do {
			neurons = await snsWrapper.listNeurons({ beforeNeuronId })
			for (let i = 0; i < neurons.length; i++) {
				totalStake += neurons[i].cached_neuron_stake_e8s
				totalNeurons += 1n;
				totalMaturity += neurons[i].maturity_e8s_equivalent
				if (totalStake == BigInt(1_000_000)) {
					totalMaturityDevs += totalMaturity
				}
				beforeNeuronId = neurons[i].id[0];
				// @ts-ignore
				console.log(uint8ArrayToHexString(neurons[i].id[0].id))
			}
		} while (neurons.length > 0);
		
		console.log("Total stake: " + totalStake)
		console.log("Total maturity: " + totalMaturity)
		console.log("Total maturity devs: " + totalMaturityDevs)
		console.log("Total neurons: " + totalNeurons)
		
		const { metadata, swapState } = snsWrapper;
		const [data, token] = await metadata({});

		console.log("SNS:", data, token, swapState);
	}

	onMount(readGovernance)
</script>
<svelte:head>
	<title>Token Economics</title>
	<meta name="description" content="Token Economics" />
</svelte:head>

<section class="w-full flex flex-col text-lg justify-center justify-items-center content-center items-center">

	<div class="flex flex-col md:w-2/3 gap-4">
		<h2 class="font-bold text-[#29ABE2]">Token Economics</h2>
		<p class="">The core of ICX token economy is centered on preventing inflation by maintaining a capped supply of 100 million tokens. To incentivize deflation and enhance the value of the network, the protocol requires the burning of tokens to utilize the dapp, thereby reducing the total supply over time. The distribution of ICX tokens is currently delineated as follows:</p>
		<ul class="list-inside space-y-4">
			<li><span class="text-[#FBB03B]">Dev Team:</span> 15% of the total supply, equating to 15 million tokens, is reserved for the development team. These tokens are vested over a span of 4 years, underscoring the team's long-term dedication to the project and synchronizing their interests with the continued evolution and success of the platform.</li>
			<li><span class="text-[#FBB03B]">Community:</span> 17% of the tokens, amounting to 17 million tokens, are held by the broader community. This allocation is devised to amplify active participation and nurture a deep-rooted sense of ownership and collaborative decision-making within the ecosystem.</li>
			<li><span class="text-[#FBB03B]">Liquidity:</span> 2% of the tokens are being used to provide liquidity, divided between Sonic and ICPSwap DEXs.</li>
			<li><span class="text-[#FBB03B]">Treasury:</span> The rest of the tokens (66%), is safeguarded in the treasury. The primary purpose of the treasury is to fortify the project's long-term resilience, facilitating future developmental strides, forging partnerships, and spearheading other essential initiatives.</li>
		</ul>
    </div>
	<div class="flex flex-col md:w-2/3 gap-4 mt-2">
		<h2 class="font-bold text-[#ED1E79]">Decentralisation</h2>
		<p class="">Every year, a portion of the treasury will be used to reward users of the dapp by distributing neurons. In this way, the DAO will become progressively more decentralized.</p>
	</div>
	<div class="flex flex-col md:w-2/3 gap-4 mt-2">
		<h2 class="font-bold text-[#F15A24]">Smallest Unit</h2>
		<p class="">Similar to satoshis in Bitcoin, a dominic (dom) is the smallest unit of the ICX token.</p><p>1 dom = 0.00000001 ICX. 1 ICX = 100,000,000 doms.</p>
	</div>
	
	<div class="flex flex-col md:w-2/3 gap-4 mt-2">
		You can track governance parameteres and follow token transactions and neuron activity in the dashboard of our SNS. 
		<A href="https://dashboard.internetcomputer.org/sns/u67kc-jyaaa-aaaaq-aabpq-cai">Open SNS Dashboard</A>
	</div>
</section>
