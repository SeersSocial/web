<script>
	import { onMount } from 'svelte';
	import { page } from '$app/stores';
	import logo from '$lib/images/icx-logo-trans.png';
	import logo3 from '$lib/images/X-Mark.png';
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
		TextPlaceholder,

		Toggle

	} from 'flowbite-svelte';
	let width = 0;
</script>
<svelte:window bind:innerWidth={width} />
<div class="relative px-2 bg-[#0E031F] text-white">
	<Navbar
		style="background:transparent; color: white;"
		navClass="bg-[#0E031F] text-white px-2 sm:px-4 py-2.5 absolute w-full z-20 top-0 left-0"
		let:hidden
		let:toggle
		color="dark"
	>
		<NavBrand href="/" class="border-none focus:outline-none hover:border-none focus:border-none">
			<!-- <img
				src={logo3}
				class="mr-3 bg-transparent w-10"
				alt=""
			/> -->
			<span class="self-center whitespace-nowrap text-5xl">&sigma;</span>
		</NavBrand>
		<NavHamburger style="background:#0E031F" on:click={toggle} class="bg-[#0E031F] border-none outline-none" btnClass="border-none outline-none text-white focus:outline-none whitespace-normal m-0.5 rounded-lg p-1.5 bg-[#0E031F] hover:bg-[#0E031F]  ml-3 md:hidden" />
		<NavUl {hidden} style="background:#0E031F"  class="bg-[#0E031F]" ulClass="p-0 bg-[#0E031F] text-white dark:text-white rounded-lg border border-[black] flex flex-col p-4 mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium">
			<NavLi on:click={() => { if (width < 1024) toggle() }} href="/" activeClass="bg-[#0E031F] text-white" nonActiveClass="bg-[#0E031F] text-white">Home</NavLi>
			<!-- <NavLi on:click={() => { if (width < 1024) toggle() }} href="/about" activeClass="bg-[#0E031F] text-white" nonActiveClass="bg-[#0E031F] text-white">About</NavLi> -->
			<NavLi on:click={() => { if (width < 1024) toggle() }} href="/tokenomics" activeClass="bg-[#0E031F] text-white" nonActiveClass="bg-[#0E031F] text-white">Token</NavLi>
		</NavUl>
	</Navbar>
</div>