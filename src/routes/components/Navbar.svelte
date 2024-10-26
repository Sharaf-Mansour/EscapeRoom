<script>
    import { AppBar } from '@skeletonlabs/skeleton';
	import {page} from "$app/stores";
    import {goto} from "$app/navigation";
</script>


<AppBar class="xl:px-44">
	<svelte:fragment  slot="lead"><img onclick={() => goto("/")} src="/logo.png" alt="Logo" class="mx-auto w-8 xl:w-11" /></svelte:fragment>
	<h1 class="hidden xl:block">Haunted</h1>
	<svelte:fragment slot="trail">
     <button onclick={() => goto("/Home")} class:active={$page.url.pathname === "/Home"}>Home</button>
     <button onclick={() => goto("/Themes")} class:active={$page.url.pathname === "/Themes"}>Themes</button>
     <button onclick={() => goto("/ContactUs")} class:active={$page.url.pathname === "/ContactUs"}>ContactUs</button>

    </svelte:fragment>
</AppBar>


<style>
    .active {
   @apply variant-filled-primary px-5 rounded-md;
 }
</style>
