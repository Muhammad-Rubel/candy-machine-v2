<script lang="ts">
  const items = [
    {
      title: "Twitter",
      link: "#",
      image: "/public/social-media-links/twitter.svg",
    },
    {
      title: "Facebook",
      link: "#",
      image: "/public/social-media-links/facebook.svg",
    },
    {
      title: "Instagram",
      link: "#",
      image: "/public/social-media-links/instagram.svg",
    },
    {
      title: "Youtube",
      link: "#",
      image: "/public/social-media-links/youtube.svg",
    },
  ];
</script>

<footer class="mt-14 pb-10">
  <div
    class="space-y-4 md:space-y-0 md:flex justify-center items-center md:space-x-6"
  >
    {#each items as item}
      <a
        href={item.link}
        class="text-[#4c83ff] flex justify-center items-center space-x-2 hover:underline"
      >
        <img src={item.image} alt="" class="h-7" />
        <span>
          {item.title}
        </span>
      </a>
    {/each}
  </div>

  <p class="text-xs text-[#7c7f7a] text-center mt-4">
    Design by <a href="!#" class="text-[#4c83ff]">Papaya</a>.
  </p>
</footer>
