<template>
  <div class="full-wrapper">
<!--  <div class="cornerbox" style="padding-top:2rem;padding-right:2rem;margin-left:auto;">
      <div class="button connectwallet">CONNECT WALLET</div>
</div>-->

<div class="row" style="margin:auto;">


    <div class="gladiators">
      <img src="~/@/assets/muscle_guy_sil.png" alt="">
    <img class="nodesktop" src="~/@/assets/fat_guy_sil.png" alt="">

    </div>

    <div class="whitelist" style="width:512px;max-width:calc(100vw - 2rem);margin:auto;"> 
     <h1 class="parallaxtop">CHICKEN GLADIATORS</h1><br>
      <h2 style="">10,000 Unique NFTs <br>Prepare for Battle in the <b>P2E</b> Arena!</h2><br>
        <div class="gladiators2">
      <img src="~/@/assets/muscle_guy_sil.png" alt="">
    <img src="~/@/assets/fat_guy_sil.png" alt="">

    </div>
     <h1 style="">OG Whitelist: <b style="color:indianred;"><br>OPEN NOW!</b></h1><br>
<p>
           Only 100 Spots Max
</p>    <br>

     <div class="button joinbutton" >JOIN WHITELIST</div>
     <br>
     <br>
     <h2>CLOSES IN: <br>
        <Countdown deadline="April 1, 2022"></Countdown>    </h2>

        <br>
        <br>
<p>
    Watch our social for further updates... 
    <br><br></p>
    
    <div style="display:flex;margin:auto;flex-flow:row;justify-content:center;">
    <a target="_blank" href="https://twitter.com/ChickenGladsNFT"><img class="socialicon" src="~/@/assets/twitter.svg" alt=""></a>
    <a target="_blank" href="https://discord.gg/hXGhBRrcMn"><img class="socialicon" src="~/@/assets/discord.svg" alt=""></a>
    
    </div>
        <br>



    </div>
    <div class="gladiators" >
    <img class="nomobile" src="~/@/assets/fat_guy_sil.png" alt="">

    </div>

    <br>
    <br>

</div>

<div class="about-text">
    </div>


    </div>
</template>

<script>
import { mapState, mapActions } from 'vuex';
import Countdown from 'vuejs-countdown'
export default {
  data() {
    return {
      form: {
        quantity: ''
      },
      modalLoginOpen: false,
      modalMakepotionOpen: false
    };
  },
 components: {
   Countdown,
    
  },
};
</script>
<style scoped>
h2{font-size:1.5rem;}
p{max-width:calc(100vw - 4rem);margin:auto;}
.parallax-card.front{
    width: max-content!important;
    height: fit-content!important;min-height:200px;}
.parallaxtoph1{text-align:center;color:white!important;font-size:4rem;}
.gladiators{width:30%;display:flex;flex-flow:wrap;
justify-content:center;}
.gladiators2{display:none;flex-flow:wrap;
justify-content:center;}
  .gladiators > img{transition:all 0.2s ease;margin:auto;max-width:100%;}
  .gladiators > img:hover{transform:scale(1.1);}  .gladiators2 > img{transition:all 0.2s ease;margin:auto;max-width:512px;}
  .gladiators2 > img:hover{transform:scale(1.1);}
.whitelist{text-align:center;}
.socialicon{width:64px;margin-left:1rem;margin-right:1rem;transition:all 0.2s ease;}
.socialicon:hover{transform:scale(1.1);}
.parallaxtop{font-size:4rem;padding-top:1rem;}  .nodesktop{display:none;}
  .row{height:100%;}

.joinbutton{padding: 1rem;
border-radius: 0.25rem;
color: black;transition:all 0.2s ease;background-color:gold;border:unset;font-size:1.5rem;box-shadow:0px 4px black,0px 4px 10px rgba(0,0,0,0.2);}
.joinbutton:hover{background-color:black;transform:scale(1.1);border:unset;font-size:1.5rem;box-shadow:0px 2px black,0px 2px 10px rgba(0,0,0,0.2);color:gold;}
.connectwallet{background-color:transparent;border:1px solid white;box-shadow:0px 2px black;color:white;margin-bottom:2rem;transition:all 0.2s ease;}
.connectwallet:hover{background-color:white;border:1px solid white;box-shadow:0px 2px black;color:black;}
@media screen and (max-width:600px) {.gladiators2{display:flex;flex-flow:wrap;
justify-content:center;}
  .nomobile{display:none;}
  .nodesktop{display:block;}h2{font-size:1rem;}
  h1{font-size:2rem!important;max-width:calc(100vw - 4rem);margin:auto;}
   .gladiators{display:none;flex-flow:row;justify-content:center;}
  .gladiators > img{margin:auto 2rem;max-height:128px;}  .gladiators2 > img{margin:auto 2rem;max-height:128px;}
  .row{flex-flow:column;}  .gladiators2{display:flex;flex-flow:row;}
.parallaxtop{transition:all 0.2s ease;padding-top:2rem;}
.parallaxtoph1{text-align:center!important;margin:auto;color:white!important;font-size:2rem!important;padding-top:40px;}

}.hasEffect {
  cursor: pointer;
}
</style>

