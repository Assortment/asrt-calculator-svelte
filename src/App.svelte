<script>
  import Calculator from "./Calculator.svelte";
</script>

<style>
  main {
    display: flex;
    min-height: 100vh;
    align-items: center;
    justify-content: center;
    background: rgb(255, 131, 110);
    background: linear-gradient(
      90deg,
      rgba(255, 131, 110, 1) 0%,
      rgba(255, 161, 112, 1) 100%
    );
  }
</style>

<main>
  <Calculator />
</main>
