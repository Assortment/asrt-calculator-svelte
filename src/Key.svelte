<script>
  export let value;
  export let type = "number";
  export let isLarge = false;
</script>

<style>
  .key {
    display: flex;
    justify-content: center;
    align-content: center;
    padding: 2rem;
    font-size: 1.4rem;
    color: #444;
    background-color: #eeeeee;
    border: 1px solid #e4e4e4;
  }

  .function {
    background-color: #e4e4e4;
    border: 1px solid #dadada;
  }

  .operation {
    color: #674837;
    background-color: #fea270;
    border: 1px solid #f59f70;
  }

  .zero {
    grid-column: span 2;
  }
</style>

<button class="key {type}{isLarge ? ' zero' : ''}">{value}</button>
