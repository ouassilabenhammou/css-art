<div class="mondriaan">
   <div class="kolom-links">
    <div></div>
    <div></div>
    <div></div>

    <div></div>
    <div></div>
    <div></div>
    <div></div>

    <div></div>
    <div></div>
    <div></div>
    
    <div></div>
    <div></div>
    <div></div>
    <div></div>

    <div></div>
    <div></div>
    <div></div>
    <div></div>

   </div>
   
   <div class="kolom-rechts"></div>
    </div>
    
    <style>
        .mondriaan {
          display: grid;
          grid-template-columns: 1fr 1fr;
          height: 300px;
          background-color: white;
  
        }
        
        .mondriaan > div{
            border: 1px solid black;
        }

        .kolom-links{
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            grid-template-rows: repeat(7, 1fr);
        }

        .kolom-links > div{
    
            background-color: white;
            border: 1px solid black;
        }

        .kolom-links > div:nth-child(1){
            background-color: blue;
            grid-column: span 3;
        }



        .kolom-links > div:nth-child(2),
        .kolom-links > div:nth-child(3){
            background-color: white;
            
        }

        .kolom-links > div:nth-child(4),
        .kolom-links > div:nth-child(6){
            background-color: white;
        }

        .kolom-links > div:nth-child(4){
            grid-column: span 1;
        }
        .kolom-links > div:nth-child(4),
        .kolom-links > div:nth-child(5){
            grid-row: span 2;
            
        }

        .kolom-links > div:nth-child(5){
            background-color: red;
            grid-column: span 2;
        }

        .kolom-links > div:nth-child(6){
            grid-row: span 2;
        }

        .kolom-links > div:nth-child(7){
            background-color: black;
            grid-row: span 2;
        }

        .kolom-links > div:nth-child(8),
        .kolom-links > div:nth-child(10){
   
            grid-column: span 1;
        }      

        .kolom-links > div:nth-child(8){
            background-color: yellow;
            grid-column: span 1;
            grid-row: span 2;
        }
        
        .kolom-links > div:nth-child(9){
            background-color: white;
            grid-column: span 2;
        }

        .kolom-links > div:nth-child(10){
            background-color: blue;
        }
        .kolom-links > div:nth-child(11),
        .kolom-links > div:nth-child(16){
            background-color: yellow;
       
        }

        .kolom-links > div:nth-child(12){
        grid-column: span 2;
        }
       
        .kolom-links > div:nth-child(14){
     background-color: red;
     grid-row: span 2;
        }

        .kolom-links > div:nth-child(15){
            background-color: blue;
            grid-column: span 3;
        }

        .kolom-links > div:nth-child(17){
            background-color: red;
            grid-column: span 3;
        }

        
    </style>
    