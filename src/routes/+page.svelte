<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
  	import { Parallax, ParallaxLayer, StickyLayer } from 'svelte-parallax';

  	import { Avatar, Button, Card, Carousel } from 'flowbite-svelte'
	import { offset } from '@popperjs/core';
	import Roadmap from './Roadmap.svelte';

	import app from '$lib/images/app.png'
	import { onMount } from 'svelte';
	
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
let days = 0;
let hours = 0;
let minutes = 0;
let seconds = 0;
let updated = false;

function updateCountdown() {
 const targetDate = new Date('2024-05-10T00:00:00').getTime(); // Set your target date/time here
  const now = new Date().getTime();
  const difference = targetDate - now;

  // Time calculations
  days = Math.floor(difference / (1000 * 60 * 60 * 24));
  hours = Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  minutes = Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60));
  seconds = Math.floor((difference % (1000 * 60)) / 1000);
}

  const onmount = () => {
    // Update the countdown every 1 second
    const intervalID = setInterval(updateCountdown, 1000);
  }

  onMount(onmount)

</script>

<svelte:head>
	<title>Seers</title>
	<meta name="description" content="Seers" />
</svelte:head>

<section class="w-full md:flex md:flex-row">
	<div class="flex flex-col gap-4 mt-2 p-4">
		<div class="text-4xl md:text-5xl font-bold text-center">
			<span class="text-white">Seers</span>
		</div>
		<div class="text-xl p-2">
			Social network for forecasters. Bet on politics, sports, tech, science and more with play money. Create your own markets. Receive airdrops. 
		</div>
		<!-- <div class="flex justify-center">
      <a href="https://oulla-fyaaa-aaaag-qa6fa-cai.ic0.app/" role="link" class="text-center font-medium focus:outline-none inline-flex items-center justify-center px-5 py-3 text-base text-white bg-purple-700 hover:bg-purple-800 dark:bg-purple-600 dark:hover:bg-purple-700 rounded-lg">Enter Demo</a>
		</div> -->
	</div>
	<!-- <div class="flex flex-col md:w-1/2 mt-4 p-4">
		<img src={app} alt="" class="rounded-lg"/>
	</div>  -->
</section>


<section class="w-full flex flex-col md:gap-8 text-xl md:text-2xl justify-center m-2 p-2">
	<div class="text-2xl font-bold text-center">
    <Button size="lg" pill href="www.boringx.ai">Testnet</Button>
  </div>
  
  <!-- <div class="grid grid-flow-col gap-5 text-center auto-cols-max justify-center">
    <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
      <span class="countdown font-mono text-5xl">
        <span >{days}</span>
      </span>
      days
    </div> 
    <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
      <span class="countdown font-mono text-5xl">
        <span>{hours}</span>
      </span>
      hours
    </div> 
    <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
      <span class="countdown font-mono text-5xl">
        <span >{minutes}</span>
      </span>
      min
    </div> 
    <div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
      <span class="countdown font-mono text-5xl">
        <span>{seconds}</span>
      </span>
      sec
    </div>
  </div> -->
</section>

<section class="w-full flex flex-row gap-8 text-2xl justify-center mt-4 p-4">
	<div class="shadow ">
		<div class="md:flex md:flex-row w-full">
			<div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-medium mb-2 text-[#29ABE2]">DAO Controlled</h3>
				Seers operates as a social network governed by a DAO. Each update to the dapp must be approved through a voting mechanism that utilizes locked SEER tokens called neurons.
      </div>
      <div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-medium mb-2 text-[#ED1E79]">Fully On-Chain</h3>
        All user data, including posts, pictures, and videos, is stored on the blockchain. This ensures that users retain ownership of their data and have control over its use.
      </div>
		</div>
	</div>
</section>


<section class="w-full flex flex-row gap-8 text-2xl justify-center mt-4 p-4">
	<div class="shadow ">
		<div class="md:flex md:flex-row w-full">
			<div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-medium mb-2 text-[#F15A24]">Crypto Primitives</h3>
				<p>In addition to common functionalities such as posts, likes, and media uploads, we offer cryptocurrency primitives, including transfers, tokenized polls, and airdrops.</p>
			</div>
      <div class="md:w-1/2 p-4 text-xl">
				<h3 class="font-medium mb-2 text-[#FBB03B]">Capped Supply</h3>
				<p>The total supply of tokens is capped at 100 million. This ensures that we will not inflate the supply; instead, we aim to genuinely reward our users.</p>
			</div>
		</div>
	</div>
</section>

<Roadmap></Roadmap>
