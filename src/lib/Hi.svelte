<script lang="ts">
  let greeting = "hi 👋";

  function changeGreeting(to: string) {
    greeting = to;
  }

  function calculateAge(birthday: string) {
    return Math.floor((new Date().valueOf() - new Date(birthday).getTime()) / 3.15576e+10);
  }
</script>

<main class="pt-40 text-center">
  <h1 class="text-5xl font-extrabold animate-bounce" on:mouseenter={ () => changeGreeting("hey stop that it tickles 😂") } on:mouseleave={ () => changeGreeting("hi 👋") }> { greeting } </h1>

  <p class="pt-5 w-96 mx-auto"> 
    I'm a { calculateAge("2012-09-02") } year old kid who enjoys
    coding because it's always been my dream to create the next
    Facebook. I'm still not there yet, but as long as I'm always
    making progress, I'm always looking forward to create
    something.
  </p>
</main>