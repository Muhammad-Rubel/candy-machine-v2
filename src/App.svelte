<script lang="ts">
  import Accordion from "./components/Accordion.svelte";

  import Feature from "./components/Feature.svelte";
  import Footer from "./components/Footer.svelte";
  import Header from "./components/Header.svelte";
  import Hero from "./components/Hero.svelte";
  import Nft from "./components/Nft.svelte";
  import SomeGenerousPeeps from "./components/SomeGenerousPeeps.svelte";
  import Talkers from "./components/Talkers.svelte";
  import Testimonial from "./components/Testimonial.svelte";
  import Ticket from "./components/Ticket.svelte";
</script>

<div class="page-border min-h-screen">
  <div class="w-full bg-white h-full">
    <div class="max-w-[1100px] mx-auto w-[90%]">
      <Header />

      <main>
        <Nft />
        <Hero />
        <Feature />
        <Talkers />
        <SomeGenerousPeeps />
        <Testimonial />
        <Accordion />
        <Ticket />
      </main>

      <Footer />
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
