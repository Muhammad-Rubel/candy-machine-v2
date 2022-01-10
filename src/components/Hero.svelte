<script lang="ts">
  import { fade } from "svelte/transition";

  const carouselPhotos = [
    "/public/hero-image-one.jpg",
    // "/public/hero-image-one.jpg",
    // "/public/hero-image-one.jpg",
    "https://picsum.photos/300/200?random=2",
    "https://picsum.photos/300/200?random=3",
  ];

  let index = 0;

  const next = () => {
    index = (index + 1) % carouselPhotos.length;
  };
</script>

<section
  class="h-48 md:h-[31rem] lg:h-[42.5rem] xl:h-[48.5rem] relative flex justify-center overflow-hidden"
>
  {#each [carouselPhotos[index]] as src (index)}
    <img
      transition:fade
      {src}
      alt=""
      class="w-full h-full absolute top-0 left-0 object-fill"
    />
  {/each}
</section>

<button
  on:click={next}
  class="w-full bg-[#1960ff] py-2 text-white font-semibold hover:bg-[#759fff] transition duration-150 ease-in-out"
  >Next!</button
>

<style>
</style>
