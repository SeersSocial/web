<script>
	import logo from '$lib/images/icx-logo-trans.png';

	import {
		Avatar,
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
	} from 'flowbite-svelte';
</script>

<div class="relative px-8 bg-black text-white">
	<Navbar
		style="background:transparent; color: white;"
		navClass="bg-black text-white px-2 sm:px-4 py-2.5 absolute w-full z-20 top-0 left-0"
	>
		<NavBrand href="/">
			<img
				src={logo}
				class="mr-3 bg-transparent w-10 h-10 rounded-full"
				alt=""
			/>
			<span class="self-center whitespace-nowrap text-xl font-semibold">ICX</span>
		</NavBrand>
		<NavHamburger  style="color:white" btnClass="bg-black hover:bg-black"/>
		<NavUl style="color:white">
			<NavLi href="/" activeClass="bg-black text-white" nonActiveClass="bg-black text-white">Home</NavLi>
			<NavLi href="/about" activeClass="bg-black text-white" nonActiveClass="bg-black text-white">About</NavLi>
		</NavUl>
	</Navbar>
</div>