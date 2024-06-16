<script lang="ts">
  let count = 0;
  import Example from "$components/ThreeDCardEffect/Example.svelte";
</script>

<h1>Counter: {count}</h1>
<button class="btn btn-primary" on:click={() => count++}>Increase</button>
<button class="btn btn-secondary" on:click={() => count--}>Decrease</button>
<button class="btn btn-accent" on:click={() => (count *= 2)}>Double</button>
<button class="btn">Button</button>
<Example />
