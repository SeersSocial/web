<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
  	import { Parallax, ParallaxLayer, StickyLayer } from 'svelte-parallax';

  	import { Avatar, Button, Card, CarouselTransition } from 'flowbite-svelte'
	import { offset } from '@popperjs/core';

	
	
	export const images = [
  {
    id: 0,
    name: "Intuitive Interface like Twitter",
    imgurl: "https://i.ibb.co/vD1T5YS/Screenshot-2023-05-15-at-13-48-44.png",
    attribution: "seers.social",
  },
  {
    id: 1,
    name: "Prediction Markets",
    imgurl: "https://i.ibb.co/RPbF56D/Screenshot-2023-05-15-at-14-39-42.png",
    attribution: "seers.social",
  },
  {
    id: 2,
    name: "User Profiles",
    imgurl: "https://i.ibb.co/QvPBZst/Screenshot-2023-05-15-at-14-45-26.png",
    attribution: "seers.social",
  },
];
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Seers: Web3 Social Network" />
</svelte:head>

<section class="w-full md:flex md:flex-row mt-14">
	<div class="flex flex-col gap-4 md:w-1/2 mt-4 p-4">
		<div class="text-4xl font-bold text-center">
			Web3 Social Network
		</div>
		<div class="text-xl p-2">
			Seers is a decentralized application (dApp) that combines the familiar look and feel of Twitter with cryptocurrency features, enabling users to engage in decentralized social media interactions while seamlessly integrating crypto-related functionalities such as tipping, prediction markets, NFT sharing, and DAO creation. 
		</div>
		<div class="flex justify-center">
			<Button size="lg"><a href="https://oulla-fyaaa-aaaag-qa6fa-cai.ic0.app/">Enter App</a></Button>
		</div>
	</div>
	<div class="flex flex-col md:w-1/2 mt-4 p-4">
		<CarouselTransition {images} loop transitionType="fade" transitionParams="{{ duration: 500 }}"  showCaptions={false} showThumbs={false} duration="5000" slideControls={false}  showIndicators={false} />
	</div>
</section>

<section class="w-full flex flex-row gap-8 text-2xl justify-center mt-8 p-8">
	<div>+10K Posts</div>
	<div>+$15K TVL</div>
	<div>+3K Users</div>
	<div>+$25K Revenue</div>
</section>


<section class="w-full flex flex-row gap-8 text-2xl justify-center mt-4 p-4">
	<div class="shadow border rounded-lg p-4">
		<div class="md:flex md:flex-row w-full">
			<div class="md:w-1/2 p-4">
				<img src="https://i.ibb.co/ByCqhQx/Screenshot-2023-05-15-at-15-31-23.png" class="rounded" />
			</div>
			<div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-bold mb-2">Weekly Rewards in ICP</h3>
				Seers is a social network that rewards your activity with weekly ICP-based rewards. Engage with the platform, like posts, and participate in the community to earn recurring tokens. It's a revolution in social media, combining connection and rewards in one place.
			</div>
		</div>
	</div>
</section>


<section class="w-full flex flex-row gap-8 text-2xl justify-center mt-4 p-4">
	<div class="shadow border rounded-lg p-4">
		<div class="md:flex md:flex-row w-full">
			<div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-bold mb-2">Prediction Markets</h3>
				<p>In Seers, you can create, resolve, and participate in prediction markets. These markets allow users to make predictions about future events, leveraging the collective wisdom of the community. By accurately predicting outcomes, users have the opportunity to win ICP tokens as a reward for their correct predictions.</p>
				<p class="mt-2">Prediction markets provide a unique avenue for discovering truth by aggregating the collective knowledge and opinions of participants, allowing us to leverage the wisdom of the crowd to make more accurate predictions and informed decisions.</p>
			</div>

			<div class="md:w-1/2 p-4">
				<img src="https://i.ibb.co/DW5WLmt/Screenshot-2023-05-15-at-15-47-16.png" class="rounded" />
			</div>
		</div>
	</div>
</section>