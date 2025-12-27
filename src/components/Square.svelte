<script>
  // Optionele props voor aanpasbaarheid
  export let color = '#6366f1'; // Standaard indigo kleur
  export let size = 120; // Standaard grootte
</script>

<div class="square" style="--color: {color}; --size: {size}px;">
</div>

<style>
  .square {
    width: var(--size);
    height: var(--size);
    background-color: var(--color);
    border-radius: 8px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    cursor: pointer;
  }

  .square:hover {
    transform: scale(1.1) rotate(5deg);
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
  }
</style>

