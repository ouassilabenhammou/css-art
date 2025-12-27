<script>
  import Square from '../components/Square.svelte';
  import Mondriaan from '../components/Mondriaan.svelte';
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<div class="layout">
  <!-- Vierkantjes container -->
<div class="squares-container">
  <Square color="#6366f1" />
  <Square color="#ec4899" />
  <Square color="#10b981" />
</div>
  <div>
<Mondriaan />
</div>
</div>


<!-- Style -->

<style>
  .squares-container {
    display: flex;
    gap: 20px;
    margin-top: 30px;

    flex-wrap: wrap;
    border: 2px solid black;
  }

  .layout{
    display: grid;
    grid-template-columns: 1fr 1fr;

  }

  @media (max-width: 768px){
    .layout{
      grid-template-columns: 1fr;
      gap: 10px;
    }
  }

</style>