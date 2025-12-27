<div class="container">
<div class="driehoek"></div>
<div class="boog">

</div>

<div class="hart">
    Dit is gemaakt met "background"
    <div class="vierkant"></div>
</div>

<div class="hart-versie-2">
    Dit is met pseudo elementen
    <div class="hartje">
    
    </div>
</div>

<div class="shaduw-effect">
    Dit is met box-shadow gemaakt
    <div class="box"></div>

</div>
<div class="rond"></div>

</div>
<style>
  .container{
   border: 1px solid black;
   display: grid;
   grid-template-columns:repeat(6, 1fr);
  }

.driehoek {
  width: 100px;
  height: 100px;
  position: relative;
  background:
    radial-gradient(circle at 40% 50%, gold 31%, transparent 31%),
    radial-gradient(circle at 40% 50%, black 40%, transparent 41%),
    linear-gradient(135deg, green 50%, transparent 50%) 0 50% / 5em 5em,
    linear-gradient(-45deg, red 50%, transparent 50%) 0 50% / 5em 5em,
    linear-gradient(grey, grey) 10px -40px / 100px 100px;
  background-repeat: no-repeat;
}

.boog {
  width: 100px;
  height: 50px;
  border: 6px solid black;
  border-bottom: none;
  border-radius: 100px 100px 0 0;
}

.hart{
    position: relative;
    width: 200px;
    height: 200px;
    border: 1px solid black;
    background: radial-gradient(circle at 50% 50%, red 31%, transparent 31%) 50% 50% / 100px 100px, 
    radial-gradient(circle at 50% 50%, red 31%, transparent 31%) 20% 50% / 100px 100px;
    background-repeat: no-repeat;
}

.vierkant {
  width: 42px;
  height: 42px;
  background-color: red;
  position: absolute;
  left: 42.5%;
  top: 58%;          
  transform: translate(-50%, -50%) rotate(45deg);
}


/* Met pseudo elementen */
.hart-versie-2{
position: relative;
width: 200px;
height: 200px;
border: 1px solid black;
}

.hartje{
  position: relative;
  width: 40px;
  height: 40px;
  background: red;
  transform: rotate(-45deg);
  top: 40%;
  left: 40%;
}


.hartje::before{
  content: "";
  position: absolute;
  width: 40px;
  height: 40px;
  background: red;
  border-radius: 50%;
  top: -20px;
  left: 0;
}


.hartje::after{
  content: "";
  position: absolute;
  width: 40px;
  height: 40px;
  background: red;
  border-radius: 50%;
  top: 0;
  left: 20px;
}

.shaduw-effect{
    display: flex;
    flex-direction: column;
 width: 200px;
 height: 200px;
 border: 1px solid black;
}

.box{
    width: 100px;
    height: 100px;
    background-color: lightgray;
    box-shadow: 
    inset 20px 10px 10px 5px grey, inset 40px 30px 10px 10px yellow;
}

.rond{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    background-color: red;
    box-shadow: 0 5px 0 red, 0 -5px 0 green, inset 0 5px 0 #ccc, inset 0 -5px 0 #ccc, inset 0 10px 0 blue, inset 0 -10px 0 blue;
    transform: rotate(-90deg);
}




</style>