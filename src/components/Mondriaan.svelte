<script>
  const items = Array(17);
</script>

<div class="mondriaan">
  <div class="kolom-links" >
    {#each items as _}
      <div ></div>
    {/each}
  </div>
  <div class="kolom-rechts"></div>
</div>
    
   <style>
  .mondriaan {
    display: grid;
    grid-template-columns: 1fr 1fr;
    height: 300px;
    background: white;
  }
         .mondriaan > div {
    border: 1px solid black;
  }

  .kolom-links {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(7, 1fr);
  }

  .kolom-links > div {
    background: white;
    border: 1px solid black;
  }

  .kolom-links > div:nth-child(1) { background: blue; grid-column: span 3; }
  .kolom-links > div:nth-child(4), .kolom-links > div:nth-child(5) { grid-row: span 2; }
  .kolom-links > div:nth-child(5) { background: red; grid-column: span 2; }
  .kolom-links > div:nth-child(6) { grid-row: span 2; }
  .kolom-links > div:nth-child(7) { background: black; grid-row: span 2; }
  .kolom-links > div:nth-child(8) { background: yellow; grid-row: span 2; }
  .kolom-links > div:nth-child(9) { grid-column: span 2; }
  .kolom-links > div:nth-child(10) { background: blue; }
  .kolom-links > div:nth-child(11), .kolom-links > div:nth-child(16) { background: yellow; }
  .kolom-links > div:nth-child(12) { grid-column: span 2; }
  .kolom-links > div:nth-child(14) { background: red; grid-row: span 2; }
  .kolom-links > div:nth-child(15) { background: blue; grid-column: span 3; }
  .kolom-links > div:nth-child(17) { background: red; grid-column: span 3; }
</style>