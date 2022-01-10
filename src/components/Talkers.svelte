<script lang="ts">
  const items = [
    {
      name: "Alyssa Long",
      image: "/public/talkers/woman1.jpg",
    },
    {
      name: "Jonathan Foster",
      image: "/public/talkers/man1.jpg",
    },
    {
      name: "Kiara Taylor",
      image: "/public/talkers/woman2.jpg",
    },
    {
      name: "Elijah Rhodes",
      image: "/public/talkers/man2.jpg",
    },
    {
      name: "Anita Gonzalez",
      image: "/public/talkers/woman3.jpg",
    },
    {
      name: "Adrian Sosa",
      image: "/public/talkers/man3.jpg",
    },
  ];
</script>

<section class="mt-20 md:mt-28">
  <h2 class="text-xl font-bold text-center md:text-2xl">The talkers</h2>

  <div
    class="mt-8 space-y-7 md:space-y-0 md:grid grid-cols-6 md:gap-x-12 md:mt-10 xl:gap-x-10"
  >
    {#each items as item}
      <div class="w-full">
        <img src={item.image} alt="" />
        <p class="text-sm mt-3 text-center">{item.name}</p>
      </div>
    {/each}
  </div>
</section>
