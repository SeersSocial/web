<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/icx-logo-trans.png';
	import github from '$lib/images/github.svg';

	import {
		Avatar,
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		ImagePlaceholder,
		Skeleton,
		TextPlaceholder
	} from 'flowbite-svelte';
</script>

<div class="relative px-8 bg-black text-white">
	<Navbar
		style="background:transparent; color: white;"
		navClass="bg-black text-white px-2 sm:px-4 py-2.5 absolute w-full z-20 top-0 left-0"
		let:hidden
		let:toggle
		color="dark"
	>
		<NavBrand href="/" class="border-none hover:border-none focus:border-none">
			<img
				src={logo}
				class="mr-3 bg-transparent w-10 h-10 rounded-full"
				alt=""
			/>
			<span class="self-center whitespace-nowrap text-xl font-semibold">ICX</span>
		</NavBrand>
		<NavHamburger style="background:black" on:click={toggle} class="" btnClass="text-white focus:outline-none whitespace-normal m-0.5 rounded-lg focus:ring-2 p-1.5 focus:ring-gray-400  bg-black hover:bg-black  ml-3 md:hidden" />
		<NavUl {hidden} style="background:black"  ulClass="bg-black dark:bg-black text-white dark:text-white rounded-lg border border-black dark:border-black flex flex-col p-4 mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium">
			<NavLi href="/" activeClass="bg-black text-white" nonActiveClass="bg-black text-white">Home</NavLi>
			<NavLi href="/about" activeClass="bg-black text-white" nonActiveClass="bg-black text-white">About</NavLi>
			<NavLi href="/tokenomics" activeClass="bg-black text-white" nonActiveClass="bg-black text-white">Token</NavLi>
		</NavUl>
	</Navbar>
</div>

<style>
	ul {
		background-color: black;
	}
</style>