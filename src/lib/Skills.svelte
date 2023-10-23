<script lang="ts">
  import { onMount } from "svelte";

  const skills = [
    "Data Science",
    "Web Development",
    "Game Development",
    "AI"
  ];

  let index = 0;

  onMount(() => {
    setInterval(() => {
      if (index === skills.length - 1) {
        index = 0;
      }
      else {
        index++;
      }
    }, 1000);
  });
</script>

<main class="pt-40 text-center">
  <h1 class="text-5xl font-extrabold animate-bounce"> skills 🎯 </h1>

  <p class="pt-5 w-96 mx-auto"> 
    Over the past few years of my coding journey, I've learned
    a lot of skills. I'm not comfortable with much of these, but
    I know:
  </p>

  <h1 class="flex justify-center pt-5 text-4xl font-bold"> { skills[index] } </h1>
</main>