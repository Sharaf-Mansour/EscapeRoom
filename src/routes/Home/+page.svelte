

<script>
        import {goto} from "$app/navigation";
</script>


<section class="">
    <div>
      <iframe
        src="https://www.youtube.com/embed/t7z4MLvSkJE?autoplay=1&rel=0&controls=1"
        title="HAUNTED ESCAPE ROOM LEBANON"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen
        class="w-full h-64 xl:h-80"
      ></iframe>
    </div>
  </section>
  
<section class=" intro flex items-center justify-center h-80 mt-5">
    <div class="text-center">
     <h2 class="h3 p-5 xl:px-56">Welcome to Haunted, where reality merges with nightmares. Dive into a world of chilling mysteries and spine-tingling puzzles that test your courage and wit. Can you uncover the dark secrets before time runs out? Enter if you dare, but beware: not all who enter Haunted make it back!</h2>
    </div>
    </section>


    <!-- how to play  -->
    <section class="Howtoplay mt-10 ">
        <h1 class="text-center h1 font-bold mt-5 mb-10">How To Play</h1>
        <div class="grid grid-cols-1 md:grid-cols-3 xl:grid-cols-3 xl:gap-2 md:gap-2">
          
          <div>
            <div class="card mb-5 h-96">
              <header>
                <img src="how1.jpg" class="w-full h-48 object-cover bg-black/50 rounded-md" alt="Post" />
              </header>
              <div class="card-header text-center">
                <h2 class="h2">Step 1</h2>
              </div>
              <div class="card-header">
                <h2 class="h5">You and your team will choose one of our cool themes. You can choose to experience the game with horror or you can play the classic escape room experience with no horror.</h2>
              </div>
            </div>
          </div>
      
          <div>
            <div class="card mb-5 h-96">
              <header>
                <img src="how2.jpg" class="w-full h-48 object-cover bg-black/50 rounded-md" alt="Post" />
              </header>
              <div class="card-header text-center">
                <h2 class="h2">Step 2</h2> <!-- Changed to Step 2 for clarity -->
              </div>
              <div class="card-header">
                <h2 class="h5">You and your team will choose one of our cool themes. You can choose to experience the game with horror or you can play the classic escape room experience with no horror.</h2>
              </div>
            </div>
          </div>
      
          <div>
            <div class="card h-96">
              <header>
                <img src="how3.jpg" class="w-full h-48 object-cover bg-black/50 rounded-md" alt="Post" />
              </header>
              <div class="card-header text-center">
                <h2 class="h2">Step 3</h2> <!-- Changed to Step 3 for clarity -->
              </div>
              <div class="card-header text-center">
                <h2 class="h5">We guarantee a fun time, can you ESCAPE?</h2>
                <br>
                <h2  onclick={() => goto("/Themes")} class="h5 cursor-pointer">See Themes => </h2>
              </div>
            </div>
          </div>
      
        </div>
      </section>
      
 
      

    <style>
        .intro {
          background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("/Home.gif");
          background-size: cover;
          background-position: center;
        }
       </style>