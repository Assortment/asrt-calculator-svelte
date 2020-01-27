<script>
  import Key from "./Key.svelte";
  import keys from "./keys";
</script>

<style>
  .calculator {
    border-radius: 1rem;
    overflow: hidden;
    box-shadow: 0 0 2rem rgba(0, 0, 0, 0.3);
  }

  .keypad {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
  }

  .display {
    padding: 5rem 1rem 1rem 1rem;
    font-size: 3rem;
    text-align: right;
    color: #ffefe7;
    background-color: #333a4e;
  }
</style>

<div class="calculator">
  <div class="display">100</div>
  <div class="keypad">
    {#each keys as { value, type, isLarge }}
      <Key {value} {type} {isLarge} />
    {/each}
  </div>
</div>
