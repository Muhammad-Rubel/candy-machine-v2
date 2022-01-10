<script lang="ts">
  const items = [
    "/public/company-logos/stripe.svg",
    "/public/company-logos/segment.svg",
    "/public/company-logos/newrelic.svg",
    "/public/company-logos/drift.svg",
    "/public/company-logos/zopim.svg",
  ];
</script>

<section class="mt-20 md:mt-28">
  <h2 class="text-xl md:text-2xl font-bold text-center tracking-wide">
    Some generous peeps
  </h2>
  <div class="mt-8 flex flex-wrap justify-center items-center md:mt-10">
    {#each items as item, i}
      <img src={item} alt="" class="m-[.8rem] {i === 2 ? 'h-10' : 'h-12'}" />
    {/each}
  </div>
</section>
