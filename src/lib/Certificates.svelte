<script lang="ts">
  import Teens from "../assets/teens.png";
  import CS50 from "../assets/cs50.png";
  import LearnToCode from "../assets/learntocode.png";
  import Web from "../assets/web.png";
</script>

<main class="pt-40 text-center">
  <h1 class="text-5xl font-extrabold animate-bounce"> certificates 🎓 </h1>

  <div class="grid grid-cols-2 gap-4 pt-5 pl-5 w-[30rem] m-auto">
    <img src="{Teens}" alt="yomama" class="h-[11.2rem]">
    <img src="{CS50}" alt="Shopping Cart Project">
    <img src="{LearnToCode}" alt="Coolgle" class="w-[13.7rem]">
    <img src="{Web}" alt="Coolgle" class="w-[13.7rem] h-[10.6rem]">
  </div>
</main>

<style scoped lang="postcss">
  img {
    @apply hover:opacity-75;
  }
</style>