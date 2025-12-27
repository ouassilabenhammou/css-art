<script>
    import Square from "$lib/components/oefenen/Square.svelte";
    import Mondriaan from "$lib/components/oefenen/Mondriaan.svelte";
  </script>
  
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
  