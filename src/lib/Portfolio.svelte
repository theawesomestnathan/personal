<script lang="ts">
  import Calculator from "../assets/calc.png";
  import Bria from "../assets/bria.png";
  import Coolgle from "../assets/coolgle.png";
</script>

<main class="pt-40 text-center">
  <h1 class="text-5xl font-extrabold animate-bounce"> portfolio 🎨 </h1>

  <div class="grid grid-cols-2 gap-4 pt-5 pl-5 w-[30rem] m-auto">
    <img src="{Calculator}" alt="yomama">
    <img src="{Bria}" alt="Shopping Cart Project">
    <img src="{Coolgle}" alt="Coolgle">
  </div>
</main>

<style scoped lang="postcss">
  img {
    @apply hover:opacity-75;
  }
</style>