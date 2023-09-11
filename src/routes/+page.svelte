<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
  	import { Parallax, ParallaxLayer, StickyLayer } from 'svelte-parallax';

  	import { Avatar, Button, Card, Carousel } from 'flowbite-svelte'
	import { offset } from '@popperjs/core';
	import Roadmap from './Roadmap.svelte';

	
	
	export const images = [
  {
    alt: "Intuitive Interface like Twitter",
    src: "https://i.ibb.co/vD1T5YS/Screenshot-2023-05-15-at-13-48-44.png",
    title: "seers.social",
  },
  {
    alt: "Prediction Markets",
    src: "https://i.ibb.co/RPbF56D/Screenshot-2023-05-15-at-14-39-42.png",
    title: "seers.social",
  },
  {
    alt: "User Profiles",
    src: "https://i.ibb.co/QvPBZst/Screenshot-2023-05-15-at-14-45-26.png",
    title: "seers.social",
  }
];
</script>

<svelte:head>
	<title>ICX: Web3 Social Network</title>
	<meta name="description" content="ICX: Web3 Social Network" />
</svelte:head>

<section class="w-full md:flex md:flex-row mt-14">
	<div class="flex flex-col gap-4 md:w-1/2 mt-4 p-4">
		<div class="text-4xl font-bold text-center">
			Web3 Social Network
		</div>
		<div class="text-xl p-2">
			ICX is a decentralized application (dApp) that combines the familiar look and feel of Twitter with cryptocurrency features, enabling users to engage in decentralized social media interactions while seamlessly integrating functionalities such as tipping, prediction markets, NFT sharing, and DAO creation. 
		</div>
		<div class="flex justify-center">
			<a href="https://oulla-fyaaa-aaaag-qa6fa-cai.ic0.app/"><Button size="lg">Enter Demo</Button></a>
		</div>
	</div>
	<div class="flex flex-col md:w-1/2 mt-4 p-4">
		<img src="https://i.ibb.co/vD1T5YS/Screenshot-2023-05-15-at-13-48-44.png" alt="screenshot"/>
	</div> 
</section>

<section class="w-full flex flex-row gap-4 md:gap-8 text-2xl justify-center mt-8 p-8">
	<div>+10K Posts</div>
	<div>+$15K TVL</div>
	<div>+3K Users</div>
	<div>+$25K Revenue</div>
</section>


<section class="w-full flex flex-row gap-8 text-2xl justify-center mt-4 p-4">
	<div class="shadow ">
		<div class="md:flex md:flex-row w-full">
			<div class="md:w-1/2 p-4">
				<img src="https://i.ibb.co/ByCqhQx/Screenshot-2023-05-15-at-15-31-23.png" class="rounded" />
			</div>
			<div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-bold mb-2">Weekly Rewards in ICP</h3>
				ICX is a social network that rewards your activity with weekly ICP/ICX tokens. Engage and contribute to earn rewards, revolutionizing the fusion of social media and token economics in one platform.
			</div>
		</div>
	</div>
</section>


<section class="w-full flex flex-row gap-8 text-2xl justify-center mt-4 p-4">
	<div class="shadow ">
		<div class="md:flex md:flex-row w-full">
			<div class="md:w-1/2 p-4">
				<img src="https://i.ibb.co/DW5WLmt/Screenshot-2023-05-15-at-15-47-16.png" class="rounded" />
			</div>
			<div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-bold mb-2">Prediction Markets</h3>
				<p>In ICX, you can create, resolve, and participate in prediction markets. These markets allow users to make predictions about future events, leveraging the collective wisdom of the community.</p> 
				<p class="pt-4">By accurately predicting outcomes, users have the opportunity to win ICP tokens as a reward for their correct predictions.</p>
				<p class="pt-4">Prediction markets are resolved using token voting and a decentralised sports oracle.</p>
			</div>
		</div>
	</div>
</section>

<Roadmap></Roadmap>