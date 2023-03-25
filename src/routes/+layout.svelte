<script lang="ts">
	import '../app.postcss';
	import { onMount } from 'svelte';
	import { DarkMode, Navbar, NavBrand, NavLi, NavUl, NavHamburger, Button } from 'flowbite-svelte';
	import {
    Footer,
    FooterBrand,
    FooterLinkGroup,
    FooterLink,
    FooterCopyright,
    FooterIcon
  } from 'flowbite-svelte';

	let breakPoint: number = 1024;
	let width: number;
	let activateClickOutside = true;
	let drawerHidden: boolean = false;
	$: if (width >= breakPoint) {
		drawerHidden = false;
		activateClickOutside = false;
	} else {
		drawerHidden = true;
		activateClickOutside = true;
	}
	onMount(() => {
		if (width >= breakPoint) {
			drawerHidden = false;
			activateClickOutside = false;
		} else {
			drawerHidden = true;
			activateClickOutside = true;
		}
	});
	let darkmodebtn =
		'text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-lg p-2.5    md:top-3 md:right-2 z-50';
	let divClass = 'w-full md:block md:w-auto';
	let ulClass =
		'flex flex-col p-4 text-center mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-lg md:font-medium';
</script>

<svelte:window bind:innerWidth={width} />

<header class="sticky top-0 z-50">
	
	<Navbar let:hidden let:toggle>
		<NavBrand href="/">
			<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white pl-4">
				Asterisc.in
			</span>
		</NavBrand>
		<div class="flex md:order-2">
		  <Button size="sm">Get started</Button>
		  <DarkMode btnClass={darkmodebtn} />

		  <NavHamburger on:click={toggle} />
		</div>
		<NavUl {hidden} {divClass} {ulClass} class="order-1">
		  <NavLi href="/" active={true}>Home</NavLi>
		  <NavLi href="/about">About</NavLi>
		  <NavLi href="/courses">Courses</NavLi>
		  <NavLi href="/faqs">FAQs</NavLi>
		  <NavLi href="/testimonials">Testimonials</NavLi>
		  <NavLi href="/contact">Contact</NavLi>
		</NavUl>
	  </Navbar>
</header>

<main>
	<slot />
</main>

<Footer footerType="socialmedia">
	<div class="mx-auto max-w-screen-xl text-center">
	  <FooterBrand
		href="https://flowbite.com"
		src="https://flowbite.com/docs/images/logo.svg"
		alt="Flowbite Logo"
		name="Flowbite"
		aClass="flex justify-center items-center text-2xl font-semibold text-gray-900 dark:text-white"
	  />
	  <p class="my-6 text-gray-500 dark:text-gray-400">
		Open-source library of over 400+ web components and interactive elements built for better
		web.
	  </p>
	  <FooterLinkGroup
		ulClass="flex flex-wrap justify-center items-center mb-6 text-gray-900 dark:text-white"
	  >
		<FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="/">About</FooterLink>
		<FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="/">Premium</FooterLink>
		<FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="/">Campaigns</FooterLink>
		<FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="/">Blog</FooterLink>
		<FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="/"
		  >Affiliate Program</FooterLink
		>
		<FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="/">FAQs</FooterLink>
		<FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="/">Contact</FooterLink>
	  </FooterLinkGroup>
	  <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400"
		>© 2021-2022 <a href="https://flowbite.com/" class="hover:underline">Flowbite™</a>. All
		Rights Reserved.</span
	  >
	</div>
  </Footer>
  