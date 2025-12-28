<script>
    
</script>
<div class="container">
    <div class="logo-wrapper">
        <div class="willemII">
            <div class="logo">
                <div class="kroon"></div>
                <div class="opening links"></div>
                <div class="opening rechts"></div>
    
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

    .kroon{
        position: absolute;
        width: 120px;
        height: 40px;
        background-color: white;
        top: -45px;
        left: 30px;
        border:5px solid var(--goud) ;
        border-top: none;
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
