<script>
	import { onMount } from 'svelte';
	import { goto } from '$app/navigation';
	var loadingindicator = $state(false) ; 
        import { ProgressRadial } from '@skeletonlabs/skeleton';
        function loading() {
          loadingindicator = true 
        }
	$effect(() => {
		AOS.init({ duration: 1000 }); // Adjust duration as needed
	});
</script>

{#if loadingindicator}
  

<div class="h-screen home flex items-center justify-center bg-black ">
	<ProgressRadial />
</div>
  
<style>
     .home{
	 display:none;
   }
</style>


{/if}
<section class="h-screen home flex items-center justify-center">
	<div class="text-center">
		<h2 data-aos="fade-right" class="h1 font-bold">Welcome to</h2>
		<h1 data-aos="fade-right" class="h1 font-extrabold">Haunted Escape Room</h1>
		<img
		    
			data-aos="fade-up"
			src="/logo.png"
			alt="Logo"
			class="mx-auto w-60 mt-3 mb-3"
			onloadeddata={loading}
		/>
		<button
			data-aos="fade-down"
			class="primary bg-primary-900 px-10 py-3 rounded-md"
			onclick={() => goto('/Home')}
		>
			Know more about us
		</button>
	</div>
</section>

<style>
	.home {
		background-image: linear-gradient(
				rgba(0, 0, 0, 0.5),
				rgba(0, 0, 0, 0.5)
			),
			url('/home2.gif');
		background-size: cover;
		background-position: center;
	}
</style>
