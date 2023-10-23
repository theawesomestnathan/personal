<script lang="ts">
  import Toggle from "./lib/Toggle.svelte";
  import Hi from "./lib/Hi.svelte";
  import Skills from "./lib/Skills.svelte";
  import Portfolio from "./lib/Portfolio.svelte";
  import Certificates from "./lib/Certificates.svelte";
  import Social from "./lib/Social.svelte";

  let page = "hi";

  function changePage(to: string) {
    page = to;
  }
</script>

<main>
  <Toggle/>

  {#if page === "hi"} 
    <Hi/>
  {:else if page === "skills"}
    <Skills/>
  {:else if page === "portfolio"}
    <Portfolio/>  
  {:else if page === "certificates"}
    <Certificates/> 
  {:else if page === "social"}
    <Social/>
  {/if}

  <div class="flex pt-10 justify-center space-x-3">
    <button on:click={() => changePage("hi")}> hi </button>
    <p> | </p>
    <button on:click={() => changePage("skills")}> skills </button>
    <p> | </p>
    <button on:click={() => changePage("portfolio")}> portfolio </button>
    <p> | </p>
    <button on:click={() => changePage("certificates")}> certificates </button>
    <p> | </p>
    <button on:click={() => changePage("social")}> socials </button>
  </div>
</main>
