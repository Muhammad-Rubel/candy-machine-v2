<script lang="ts">
  import Feature from "./components/Feature.svelte";
  import Header from "./components/Header.svelte";
  import Hero from "./components/Hero.svelte";
  import Nft from "./components/Nft.svelte";
  import Talkers from "./components/Talkers.svelte";
</script>

<div class="page-border min-h-screen">
  <div class="w-full bg-white h-full ">
    <div class="max-w-[1100px] mx-auto">
      <Header />

      <main>
        <Nft />
        <Hero />
        <Feature />
        <Talkers />
      </main>
    </div>
  </div>
</div>

<style>
  .page-border {
    padding: 0.8rem;
    background-color: #2afadf;
    background-image: linear-gradient(135deg, #2afadf 10%, #4c83ff 100%);
  }

  @media only screen and (min-width: 600px) {
    .page-border {
      padding: 1.8rem;
    }
  }
</style>
