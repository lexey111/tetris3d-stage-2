<script lang="ts">
  import Next from "./components/Next.svelte";

  const figures = "SZLJITO".split("");
  let figure = "";

  setInterval(() => {
    figure = figures[Math.floor(Math.random() * figures.length)];
  }, 500);
</script>

<main>
  <Next {figure} />
</main>

<style>
  /* nothing yet here */
</style>
