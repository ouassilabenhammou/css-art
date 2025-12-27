<script>
  import Square from '../components/Square.svelte';
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<div class="squares-container">
  <Square color="#6366f1" />
  <Square color="#ec4899" />
  <Square color="#10b981" />
</div>

<style>
  .squares-container {
    display: flex;
    gap: 20px;
    margin-top: 30px;
    flex-wrap: wrap;
  }
</style>