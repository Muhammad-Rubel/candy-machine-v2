<script lang="ts">
  // import Accordion from "svelte-accordion";
  import { slide } from "svelte/transition";
  type numOrNull = null | number;
  let expandedItem: numOrNull = null;
  const items = [
    {
      title: "Header One",
      details:
        "No matter what has happened to you in the past or what is going on in your life right now, it has no power to keep you from having an amazingly good future if you will walk by faith in God. God loves you! He wants you to live with victory over sin so you can possess His promises for your life today!",
    },
    {
      title: "Header Two",
      details:
        "No matter what has happened to you in the past or what is going on in your life right now, it has no power to keep you from having an amazingly good future if you will walk by faith in God. God loves you! He wants you to live with victory over sin so you can possess His promises for your life today!",
    },
    {
      title: "Header Three",
      details:
        "No matter what has happened to you in the past or what is going on in your life right now, it has no power to keep you from having an amazingly good future if you will walk by faith in God. God loves you! He wants you to live with victory over sin so you can possess His promises for your life today!",
    },
  ];

  const expand = (i: number) => {
    if (expandedItem === i) {
      expandedItem = null;
    } else {
      expandedItem = i;
    }
  };
</script>

<section class="mt-20 md:mt-28">
  <div class="space-y-1">
    {#each items as item, i}
      <div
        class="flex justify-start items-center space-x-2 border bg-gray-50 cursor-pointer px-4 py-2"
        on:click={() => {
          // expandedItem = i;
          expand(i);
        }}
      >
        <img
          src="/caret-up-solid.svg"
          alt=""
          class="w-4 transform transition duration-150 ease-in-out {expandedItem ===
          i
            ? 'rotate-180'
            : 'rotate-0'}"
        />
        <h1 class="font-bold">
          {item.title}
        </h1>
      </div>
      {#if expandedItem === i}
        <p transition:slide class="text-left px-4 py-2 pb-4">{item.details}</p>
      {/if}
    {/each}
  </div>
</section>
