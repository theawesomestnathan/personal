<script lang="ts">
  import { Icon, Sun, Moon } from "svelte-hero-icons";

  let mode = "light";

  function toggle() {
    document.body.classList.toggle("dark");
    mode = mode === "dark" ? "light" : "dark";
  }
</script>

<main class="flex justify-end pr-1 pt-2">
  <button on:click={toggle} class="w-14 text-yellow-400">
    {#if mode === "light"}
      <Icon src="{Sun}" solid/>
    {:else if mode === "dark"}
      <Icon src="{Moon}" solid/>
    {/if}
  </button>
</main> 

<style global>

</style>