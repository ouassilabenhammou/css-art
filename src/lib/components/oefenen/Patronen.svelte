<script>
    const patroon = Array.from({ length: 4 });
    const vierkant = Array.from({ length: 5 });
  </script>
  

  
  <div class="rij">
    {#each vierkant as _}
      <div class="vierkant">
        {#each patroon as __}
          <span></span>
        {/each}
      </div>
    {/each}
  </div>

  <div class="container">
    <div class="cirkel"></div>
    <div class="cirkel-lagen"></div>
   
      
  </div>
  

  <style>
    .container{
        display: flex;
    }
    
  .cirkel {
    width: 200px;
    height: 200px;
    background: grey;
    border-radius: 50%;
    position: relative;
    margin-bottom: 40px;
  }
  
  .cirkel::before,
  .cirkel::after {
    content: "";
    position: absolute;
    border-radius: 50%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  
  .cirkel::before {
    width: 100px;
    height: 100px;
    background: black;
  }
  
  .cirkel::after {
    width: 50px;
    height: 50px;
    background: red;
  }


/* 1em = 16px */
.cirkel-lagen {
  position: absolute;
  width: 500px;
  height: 200px;
  background:
  radial-gradient(ellipse at 50% 50%, green 40%, transparent 10%) 50% 50% / 5em 5em,
  radial-gradient(circle at 50% 50%, white 40%, transparent 10%) 50% 50% / 6em 6em,  
  radial-gradient(circle at 50% 50%, green 40%, transparent 10%)50% 50% / 7em 7em,
  radial-gradient(circle at 50% 50%, white 40%, transparent 10%) 50% 50% / 8em 8em,
  radial-gradient(circle at 50% 50%, green 40%, transparent 10%) 50% 50% / 9em 9em;
  background-repeat: no-repeat;
}

  
  .rij {
    display: flex;

  }
  

  .vierkant {
    position: relative;
    width: 100px;
    height: 100px;
    background: red;
  
  }
  
  .vierkant span {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 50px;
    height: 50px;
    background: orange;
    border-radius: 100% 0 100% 0;
    transform-origin: 0 0px;
    
  }
  
  .vierkant span:nth-child(1) { transform: rotate(0deg); }
  .vierkant span:nth-child(2) { transform: rotate(90deg); }
  .vierkant span:nth-child(3) { transform: rotate(180deg); }
  .vierkant span:nth-child(4) { transform: rotate(270deg); }

  





  </style>
  