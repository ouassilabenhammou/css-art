<div class="container">
<div class="viskom-wrapper">
<div class="viskom">
    <div class="inhoud"></div>
    <div class="vissen">
        <div class="vinnen"></div>
    </div>
</div>
</div>
</div>

<style>

.container{
    --licht-blauw: #46C0F4;
    --donker-blauw: #4D85FF;
    --geel: #FFDC27;
    --donker-geel: #FFC300;
    --oranje: #FF7C2A;
    --groen: #3CCC76;
    --bg-color: #FFE8E0;
    --shaduw-color: #F4D7D1;
    --zalm-rood: #FF5E52;

    display: flex;
    justify-content: center;
    align-items: center;
    background-color: var(--bg-color);
}

.viskom-wrapper{
    position: relative;
    width: 250px;
    height: 410px;
    padding-top: 25px;
}

/* Viskom */

.viskom{
    position: relative;
    width: 250px;
    height: 250px;
    background-color: #ffffff80;
    border-radius: 50%;
    background: linear-gradient(
        to bottom,
        rgba(255, 255, 255, 0.5) 0,
        rgba(255, 255, 255, 0.5) 26%,
        var(--donker-blauw) 26%,
        var(--donker-blauw) 73%,
        var(--donker-geel) 73%,
        var(--donker-geel) 100%
    );
    z-index: 1;
}

.viskom::before{
    content: "";
    position: absolute;
    width: 100px;
    height: 10px;
    border: 10px solid white;
    border-radius: 100%;
    top: 0;
    left: 65px;
}


/* Voetstuk van de kom */

.viskom-wrapper::before{
    content: "";
    position: absolute;
    width: 110px;
    height: 40px;
    background: white;
    border-radius: 100%;
    bottom: 0;
    top: 255px;
    left: 70px;
    box-shadow:inset 0 5px 10px #0000001a;
    z-index: 1;
}

.viskom-wrapper::after{
    content: "";
    position: absolute;
    width: 200px;
    height: 60px;
    background: var(--shaduw-color);
    border-radius: 100%;
    bottom: 0;
    top: 255px;
    left: 25px;
    z-index: 0;
}

.inhoud{
    width: 219px;
    height: 30px;
    background-color: var(--licht-blauw);
    margin: 0 auto;
    border-radius: 100%;
    position: relative;
    top: 50px;
    box-shadow: 0 120px 0 var(--geel);
}

.inhoud::before{
    content: "";
    position: absolute;
    width: 60px;
    height: 10px;
    background-color: var(--donker-geel);
    border-radius: 100%;
    top: 130px;
    left: 20px;
    box-shadow: 120px 0px 0px -2px var(--donker-geel);
}   

.inhoud::after{
    content: "";
    position: absolute;
    width: 10px;
    height: 90px;
    background-color: var(--groen);
    border-radius: 10px 10px 5px 5px;
    top: 45px;
    left: 90px;
    box-shadow: 
        15px 10px 0px var(--groen), 
        30px 0px 0px var(--groen);
}  

.vissen{
    position: absolute;
    width: 60px;
    height:60px;
    background-color: var(--oranje);
    border-radius: 50%;
    top: 100px;
    left: 30px;
    box-shadow: 130px 0px 0 var(--oranje);
}

.vissen::before{
    content: "";
    position: absolute;
    width: 7px;
    height: 7px;
    background-color: black;
    border-radius: 50%;
    top: 25px;
    left: 10px;
    box-shadow: 
        20px 0px 0 black, 
        130px 0px 0 black, 
        150px 0px 0 0 black, 
        10px 15px 0 1px var(--zalm-rood), 
        10px 15px 0 5px var(--geel),
        140px 15px 0 1px var(--zalm-rood), 
        140px 15px 0 5px var(--geel)
}

.vinnen{
    position: absolute;
    width: 15px;
    height: 10px;
    top: 0px;
    left: 45px;
    border-radius: 0px 10px 0px 10px;
    transform: rotate(20deg);
    box-shadow: 
        15px 40px 0  var(--oranje),
        140px -5px 0 var(--oranje)
}

</style>