<script lang="ts">
  const items = [
    {
      icon: "/feature-icons/bucket.svg",
      details:
        "Equidem soleo etiam quod uno Graeci, si aliter non possum idem pluribus.",
    },
    {
      icon: "/feature-icons/flask.svg",
      details:
        "Nonne videmus quanta perturbatio rerum omnium consequatur quanta.",
    },
    {
      icon: "/feature-icons/aircraft.svg",
      details:
        "Hoc enim constituto in philosophia constituta sunt omnia aliter possum.",
    },
  ];
</script>

<section
  class="pt-16 space-y-4 md:flex justify-between items-start md:space-y-0 md:space-x-8"
>
  {#each items as item}
    <div class="w-full">
      <img src={item.icon} alt="" class="h-7 lg:h-8" />
      <p class="mt-2 lg:mt-4 text-left lg:text-xl">
        {item.details}
      </p>
    </div>
  {/each}
</section>
