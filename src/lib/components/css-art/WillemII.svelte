<div class="container">
<div class="logo-wrapper">
<div class="willemII">
    <div class="logo">
        <div class="kroon">
            <div>
                <div class="kroon-boog"></div>
                <div class="kroon-boog"></div>
                <div class="kroon-boog"></div>
                <div class="kroon-boog"></div>
            </div>
            <div>
                <div class="streep"></div>
                <div class="streep"></div>
                <div class="streep"></div>
                <div class="streep"></div>
                <div class="streep"></div>
            </div>

        </div>
            <div class="opening links"></div>
            <div class="opening rechts"></div>

        <div class="letter-w">
            <div class="w-streep"></div>
            <div class="w-streep"></div>
            <div class="w-streep"></div>
            <div class="w-streep"></div>
            <div class="w-streep"></div>
            <div class="w-streep"></div>
        </div>
        <div class="streepje"></div>
        
    </div>
        <div class="bal">
            <div class="boog"></div>
            <div class="boog"></div>
            <div class="boog"></div>
            <div class="boog"></div>
            <div class="boog"></div>
            <div class="boog"></div>
            <div class="boog"></div>
            <div class="boog"></div>
        </div>
</div>
</div>

</div>

<style>
.container{
    --blauw: #09294E;
    --bg-blauw: #192854;
    --rood: #C5000B;
    --goud: #D18E00;
    background-color: var(--bg-blauw);
    display: flex;
    justify-content: center;
    align-items: center;

}


.logo-wrapper{
    position: relative;
    width: 250px;
    height: 410px;
    display: flex;
    align-items: center;
    justify-content: center;
}


.willemII{
    position: relative;
    width: 190px;
    height: 215px;
    background: 
    linear-gradient(
        to bottom, 
        var(--rood) 0%, 
        var(--rood) 38%,
        white 38%,
        white 70%,
        var(--blauw) 70%, 
        var(--blauw) 100%);
    border: 5px solid var(--goud);
    border-radius: 0% 0% 10% 10%;
}   
.willemII::before{
    content: "";
    position: absolute;
    width: 150px;
    height: 15px;
    background-color: var(--blauw);
    top: 215px;
    left: 15px;
    border-radius: 0 0 20px 20px ;
    border: 5px solid var(--goud);
    border-top: none;
}


.logo::after{
    content: "18";
    font-family: 'Times New Roman', Times, serif;
    font-size: 32px;
    color: var(--goud);
    position: absolute;
    bottom: 10px;  
    left: 15px;
    transform: rotate(20deg);
}
.logo::before{
    content: "96";
    font-family:'Times New Roman', Times, serif;
    font-size: 32px;
    color: var(--goud);
    position: absolute;
    bottom: 10px;  
    left: 140px;
    transform: rotate(-20deg);
}

/* Kroon */

.kroon{
    position: absolute;
    width: 210px;
    height: 40px;
    top: -45px;
    left: -10px;
    background:
        linear-gradient(235deg, white 70%, transparent 70%) left,
        linear-gradient(-235deg, white 70%, transparent 70%) right;
    background-size:
        50% 100%;
    background-repeat: no-repeat;

}

.kroon::before{
    content: "";
    position: absolute;
    width: 10px;
    height: 10px;
    background-color: var(--goud);
    border-radius: 50%;
    top: -4px;
    left: 2px;
    z-index: 1;
    box-shadow: 
    44px -10px 0 var(--goud),
    98px -13px 0 var(--goud),
    150px -11px 0 var(--goud),
    192px -2px 0 var(--goud)
    ;
}
.streep{
    position: absolute;
    width: 5px;
    height: 50px;
    background-color: var(--goud);
    left: 102px;
    top: -5px;
    z-index: 1;
}

.streep:nth-child(2){
    left: 25px;
    top: -1px;
    transform: rotate(-40deg);
}
.streep:nth-child(3){
    left: 63px;
    top: -3px;
    transform: rotate(-30deg);
}
.streep:nth-child(4){
    left: 142px;
    top: -5px;
    transform: rotate(25deg);
}
.streep:nth-child(5){
    left: 179px;
    top: -2px;
    transform: rotate(35deg);
}


.kroon-boog{
    content:"";
    position: absolute;
    width: 30px;
    height: 30px;
    border-radius: 0% 0% 100% 0%;
    background-color:var(--bg-blauw);
    top: -16px;
    left: 15px;
    border: 5px solid var(--goud) ;
    border-top: none;
    border-left: none;
    transform: rotate(35deg) ;
}
.kroon-boog:nth-last-child(2){
    width: 35px;
    height: 35px;
    top: -23px;
    left: 59px;
    transform: rotate(41deg);
}
.kroon-boog:nth-last-child(3){
    width: 35px;
    height: 35px;
    top: -24px;
    left: 109px;
    transform: rotate(49deg);
}
.kroon-boog:nth-last-child(4){
    width: 27px;
    top: -18px;
    left: 158px;
    transform: rotate(60deg);
}




.opening{
    position: absolute;
    width: 35px;
    height: 35px;
    border-radius: 0% 0% 100% 0%;
    background-color: var(--bg-blauw);
    top: -5px;
    border:5px solid var(--goud) ;
    border-top: none;
    border-left: none;
}
.opening.links{
    left: -5px;
}
.opening.rechts{
    left: 155px;
    transform: scale(-1,1);
}


/* De letter W */

.letter-w{
    position: absolute;
   
    background-color: var(--goud);
    top: 50px;
    left: 30px;
}
.w-streep{
    position: absolute;
    width: 10px;
    height: 115px;
    background-color: var(--goud);
    top: 0px;
    left: 35px;
}

.w-streep:nth-last-child(2){
    left: 15px;
    transform: rotate(-20deg);
}
.w-streep:nth-last-child(3){
    left: 80px;
}

.w-streep:nth-last-child(4){
    left: 100px;
    transform: rotate(20deg);
}

.w-streep:nth-last-child(5){
    height: 71px;
    width: 8px;
    top: 45px;
    left: 49px;
    transform: rotate(20deg);
    background: linear-gradient(-20deg, var(--goud) 80%, transparent 80%) right;
}

.w-streep:nth-last-child(6){
    height: 71px;
    width: 8px;
    top: 45px;
    left: 68px;
    transform: rotate(-20deg);
    background: linear-gradient(20deg, var(--goud) 80%, transparent 80%) left;

}

.streepje{
    position: absolute;
    width: 30px;
    height: 5px;
    background-color: var(--goud);
    top: 50px;
    left: 15px;
    box-shadow: 40px 0 0 var(--goud), 85px 0 0  var(--goud), 125px 0 0  var(--goud);
}





/* Bal */

.bal{
    position: absolute;
    width: 80px;
    height: 80px;
    background-color: var(--goud);
    border: 4px solid var(--goud);
    border-radius: 50%;
    top: 180px;
    left: 50px;
    box-shadow: 0 0 0 var(--goud);
}

/* Bogen in de bal */

.boog{
    position: absolute;
    width: 35px;
    height: 30px;
    border-radius: 0% 0% 100% 0%;
    background-color:transparent;
    top: 19px;
    left: 0px;
    border:5px solid var(--blauw) ;
    border-top: none;
    border-left: none;
    transform: rotate(135deg) ;
    z-index: 0;
}

.boog:nth-child(1){
    width: 25px;
    height: 25px;
    top: 21px;
    left: 26px;
    transform: rotate(145deg) ;
}

.boog:nth-child(2), .boog:nth-child(3){
    width: 30px;
    height: 30px;
    top: 37px;
    left: 0px;
    transform: rotate(45deg) ;
}

.boog:nth-child(3){
    height: 35px;
    left: 16px;
    top: 52px;
    transform: rotate(35deg) ;
}

.boog:nth-child(4), .boog:nth-child(5){
    width: 35px;
    height: 35px;
    left: 43px;
    top: 34px;
    transform: rotate(50deg) ;
}

.boog:nth-child(5){
    top: 14px;
    transform: rotate(50deg) ;
}

.boog:nth-child(6){
    width: 50px;
    height: 40px;
    top: -13px;
    left: 11px;
    transform: rotate(-130deg);

}

.boog:nth-child(7){
    width: 70px;
    height: 20px;
    background-color: transparent;
    top: -6px;
    left: 5px;
    border-radius: 90px 0px 10px 0 ;
    border: 5px solid var(--blauw);
    border-bottom: none;
    transform: rotate(-163deg);
}


</style>
