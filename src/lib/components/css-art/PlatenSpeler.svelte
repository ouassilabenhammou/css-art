<div class="container">
    <div class="platenspeler-wrapper">
    <div class="platen-speler">
        <div class="plaat">
        </div>
        <div class="toonarm">
        <div class="stylus"></div>
        </div>   
    </div>
    </div>
</div>

<style>

    /* Kleuren */

    .container{
        --licht-blauw: #BEEFFF;
        --schaduw-blauw: #87E0FE;
        --rood: #D60026;
        --shaduw-rood: #820015;
        --grijs: #373232;
        --donker-grijs: #1A1A1A;
        --licht-grijs: #D9D9D9;
        --shaduw-grijs: #C2C2C2;

        display: flex;
        justify-content: center;
        align-items: center;
        background-color: var(--licht-blauw);
    }
    .platenspeler-wrapper{
        position: relative;
        width: 250px;
        height: 300px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    /* Vinly plaat */
    
    .platen-speler{
        position: relative;
        width: 250px;
        height: 150px;
        background-color: var(--rood);
        border-radius: 10px;
        box-shadow: 0 5px 0 var(--shaduw-rood);
        z-index: 3;
    }

    .platen-speler::before{
        content: "";
        position: absolute;
        width: 25px;
        height: 5px;
        background-color: black;
        box-shadow: 30px 0 0 black;
        top: 101%;
        left: 65%;
    }

    .platen-speler::after{
        content: "";
        position: absolute;
        width: 15px;
        height: 15px;
        border-radius: 50%;
        top: 60%;
        left: 85%;
        background-color: black;
        box-shadow: 0 25px 0 black;
    }

    .plaat{
        position: absolute;
        width: 162px;
        height: 162px;
        background-color: black;
        border-radius: 50%;
        top: -5px;
        left: -5px;
        z-index: -10;
        box-shadow:
            inset 0 0 0 6px black,
            inset 0 0 0 7px var(--donker-grijs),

            inset 0 0 0 12px black,
            inset 0 0 0 13px var(--donker-grijs),

            inset 0 0 0 18px black,
            inset 0 0 0 19px var(--donker-grijs),

            inset 0 0 0 24px black,
            inset 0 0 0 25px var(--donker-grijs),

            inset 0 0 0 30px black,
            inset 0 0 0 31px var(--donker-grijs);

        animation: draai-plaat 10s linear infinite;
       
    }

    .plaat::before, .plaat::after{
        content: "";
        position: absolute;
        transform: translate(-50%, -50%);
        top: 50%;
        left: 50%;
    }

    .plaat::before{
        width: 50px;
        height: 50px;
        background: linear-gradient(var(--licht-blauw) 50%, white 50%);
        box-shadow: inset 0 0 0 3px white, inset 0 0 0 4px var(--grijs), inset 0 0 0 6px white;
        border-radius: 70%;
    }

    .plaat::after{
        width: 8px;
        height: 8px;
        background-color: black;
        box-shadow:  0 0 0 2px white;
        border-radius: 50%;
    }


/* Toonarm */

.toonarm{
    position: absolute;
    width: 30px;
    height: 30px;
    background-color: black;
    border-radius: 50%;
    box-shadow: inset 0 0 0 7px var(--grijs);
    left: 75%;
    top: 10%;
}

.toonarm::before{
    content: "";
    position: absolute;
    width: 8px;
    height: 60px;
    background-color: white;
    z-index: -1;
    transform: rotate(28deg);
    top: 15px;
    left: -3px;

}
.toonarm::after{
    content: "";
    position: absolute;
    width: 8px;
    height: 40px;
    background-color: white;
    z-index: -10;
    transform: rotate(64deg);
    border-radius: 0 0 20px 20px;
    top: 58px;
    left: -33px;
}

.stylus{
    position: absolute;
    width: 9px;
    height: 8px;
    background-color: var(--licht-blauw);
    box-shadow: inset 1px 0 0 0 var(--schaduw-blauw);
    transform: rotate(65deg);
    top: 82px;
    left: -50px; 

}
.stylus::before{
    content: "";
    position: absolute;
    width: 15px;
    height: 20px;
    background-color: var(--licht-grijs);
    box-shadow: inset 3px 0 0 0 var(--shaduw-grijs);
    top: 8px;
    left: -3px;
    clip-path: polygon(0 0, 100% 0, 80% 100%, 20% 100%);
}

.stylus::after{
    content: "";
    position: absolute;
    width: 2px;
    height: 2px;
    border-radius: 50%;
    background-color: darkgray;
    top: 23px;
    left: 1px;
    box-shadow:4px 0 0 0 darkgray;
}

/* Animatie: draaiende plaat */

@keyframes draai-plaat {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}
</style>




