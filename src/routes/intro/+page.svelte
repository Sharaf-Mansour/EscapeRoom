<script>
  import { goto } from "$app/navigation";

  $effect(() => {
    AOS.init({ duration: 1000 }); // Adjust duration as needed
  });
</script>

<section class="h-screen w-screen home flex items-center justify-center">
  <div class="text-center">
    <h2 data-aos="fade-right" class="h1 font-bold">Welcome to</h2>
    <h1 data-aos="fade-right" class="h1 font-extrabold">Haunted Escape Room</h1>
    <img
      data-aos="fade-up"
      src="/logo.png"
      alt="Logo"
      class="mx-auto w-60 mt-3 mb-3"
    />
    <button
      data-aos="fade-down"
      class=" bg-yellow-300 px-10 py-3 rounded-md text-black"
      onclick={() => goto("/Home")}
    >
      Know more about us
    </button>
  </div>
</section>

<style>
  .home {
    background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
      url("/home2.gif");
    background-size: cover;
    background-position: center;
  }
</style>
