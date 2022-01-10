<script lang="ts">
  const items = [
    {
      name: "Randy Johnson",
      details: "This conference changed my life because I found my wife there.",
    },
    {
      name: "Jill Carson",
      details:
        "It takes a really long time to get to this event. Worth it? Maybe.",
    },
    {
      name: "Chase Harrop",
      details:
        "Sometimes I like to be glamorous. It makes me feel good inside.",
    },
  ];
</script>

<div class="mt-20 md:mt-28">
  <h2 class=" text-2xl font-bold text-center tracking-wide">On the record</h2>
  <div
    class="mt-8 space-y-6 md:space-y-0 md:grid grid-cols-3 md:gap-x-12 md:mt-10 xl:gap-x-10"
  >
    {#each items as item}
      <div class="w-full">
        <p class="text-left tracking-wide">{item.details}</p>
        <p class="font-bold text-left tracking-wide">> {item.name}</p>
      </div>
    {/each}
  </div>
</div>
