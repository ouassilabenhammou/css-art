<script>
   const itemsLinks = Array(19);
  const itemsRechts = Array(17);
</script>

<div class="mondriaan">
  <div class="kolom-links" >
      {#each itemsLinks as _}
      <div ></div>
    {/each}
  </div>
  <div class="kolom-rechts">
    {#each itemsRechts as _}
    <div ></div>
  {/each}
  </div>
</div>
    
   <style>
  .mondriaan {
    display: grid;
    grid-template-columns: 1fr 1fr;
    height: 300px;
    border:solid black;
    height: 500px;
    background: white;
  }

  .mondriaan > div {
    border: 1px solid black;
  }
 .kolom-links, .kolom-rechts{
    display: grid;
   grid-template-columns: repeat(6, 1fr);
    grid-template-rows: repeat(10, 1fr);
  }

 .kolom-links > div, .kolom-rechts > div {
    background: white;
    border: solid black;

  }
 .kolom-links > div:nth-child(1) { background: blue; grid-column: span 4; }
  .kolom-links > div:nth-child(4), 
  .kolom-links > div:nth-child(5), 
  .kolom-links > div:nth-child(6), 
  .kolom-links > div:nth-child(11){ grid-row: span 2; }

  .kolom-links > div:nth-child(5) { background: red; grid-column: span 3; }
  .kolom-links > div:nth-child(7) { background: black; grid-row: span 2; }
  
  .kolom-links > div:nth-child(8) { background: yellow; grid-row: span 4; }
  .kolom-links > div:nth-child(9),   
  .kolom-links > div:nth-child(12) { grid-column: span 3; grid-row: span 2; }

  .kolom-links > div:nth-child(10) { background: blue; grid-row: span 2;}
  .kolom-links > div:nth-child(14) { background: red; grid-row: span 4; }
  .kolom-links > div:nth-child(15) { background: blue; grid-column: span 3; grid-row: span 2;}
  .kolom-links > div:nth-child(16) {background-color: yellow; grid-column: span 2;}

  .kolom-links > div:nth-child(17) { background: red; grid-column: span 3; }
 .kolom-links > div:nth-child(18) { grid-column: span 2;}


  .kolom-rechts > div:nth-child(1)  { grid-column: span 4; }
  .kolom-rechts > div:nth-child(2),
  .kolom-rechts > div:nth-child(6),
  .kolom-rechts > div:nth-child(9),
  .kolom-rechts > div:nth-child(13),
  .kolom-rechts > div:nth-child(15) { grid-row: span 2; }

  .kolom-rechts > div:nth-child(2)  { background: yellow; }
  .kolom-rechts > div:nth-child(3)  { background: black; }
  .kolom-rechts > div:nth-child(4),
  .kolom-rechts > div:nth-child(5)  { grid-column: span 2; grid-row: span 2; }

  .kolom-rechts > div:nth-child(5),
  .kolom-rechts > div:nth-child(10) { background: red; }

  .kolom-rechts > div:nth-child(9){background-color: blue;}
  .kolom-rechts > div:nth-child(10) {grid-row: span 4; }

  .kolom-rechts > div:nth-child(8)  { grid-column: span 4; grid-row: span 2; }
  .kolom-rechts > div:nth-child(11) { background: blue; grid-column: span 4; grid-row: span 2; }
  .kolom-rechts > div:nth-child(12) { grid-column: span 3; grid-row: span 2; }
  .kolom-rechts > div:nth-child(14) { grid-row: span 3; }
  .kolom-rechts > div:nth-child(16) { background: black; grid-column: span 4; }
  .kolom-rechts > div:nth-child(17) { background: blue; }

</style>