<script>
	import '../app.postcss';
	import {browser} from "$app/environment";
	import { ProgressRadial } from '@skeletonlabs/skeleton';
	import Navbar from './components/Navbar.svelte';
	import Footer from './components/footer.svelte';
	import {page} from "$app/stores";
	let { children } = $props();
</script>

{#if !browser}

<div class="h-screen home flex items-center justify-center bg-black ">
	<ProgressRadial />
</div>
  
  
  <style>
   .body{
	 display:none;
   }
  </style>
 {:else}
 <div class="body">
	<div class:active={$page.url.pathname === "/"}>
		<Navbar/>
	</div>

	<div class="flex flex-row justify-center">
		{@render children()}
	</div>


	<div class:active={$page.url.pathname === "/"}>
		<Footer/>
	</div>
</div>

{/if} 

<style>
	 .active {
    @apply hidden;
  }
</style>

