<template>
  <div class="full-wrapper">
  <div class="cornerbox" style="padding-top:2rem;padding-right:2rem;margin-left:auto;">
      <div class="button">CONNECT WALLET</div>
</div>
<jj-parallax-card class="parallaxtop" lightColor="transparent" style="margin:auto; width: 712px; max-width:calc(100vw - 2rem;);height: 200px;" @click="click">
      <div slot="front">
      <h1 class="parallaxtoph1">CHICKEN GLADIATORS</h1>
      <h2 style="text-align:center;">10,000 Unique Generative NFT's</h2>
      <h2 style="text-align:center;">Prepare for Battle in the <b>P2E</b> Arena!</h2>
      <!--
      <img src="~/@/assets/kappa-36.png" width="512px;" height="512px;" class="img-top" alt="">
      -->
      </div>
</jj-parallax-card>

<div class="row">


    <div class="gladiators">
      <img src="~/@/assets/muscle_guy_sil.png" alt="">

    </div>

    <div class="whitelist" style="width:512px;min-width:512px;"> 
    
     <h1 style="font-size:1.5rem;">OG Whitelist: OPEN NOW!</h1>
     <br>   

     <div class="button"><h2>JOIN WHITELIST</h2></div>
    <br>
     <br>
     <h2>CLOSES IN: <br>
        <Countdown deadline="April 1, 2022"></Countdown>
    </h2>
    
    <div style="display:flex;margin:auto;">
    <a target="_blank" href="https://twitter.com/ChickenGladsNFT "><img style="width:128px;" src="~/@/assets/twitter.svg" alt=""></a>
    <a target="_blank" href="https://discord.gg/d9MqkSG6 "><img style="width:128px;" src="~/@/assets/discord.svg" alt=""></a>
    
    </div>
    <h2>More To Come!</h2>
    <p>
    Watch our social for further updates... 
    <br><br>
    </p>
    <ul>
    <li>Contests</li>
    <li>Roadmap</li>
    <li>Gitbook</li>
    <li>Gallery</li>
    <li>and More...</li>
    </ul>


    </div>
    <div class="gladiators">
    <img src="~/@/assets/fat_guy_sil.png" alt="">

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
import JJParallaxCard from 'jj-parallax-card'
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
  'jj-parallax-card':JJParallaxCard,
    
  },
};
</script>
<style scoped>
h2{font-size:1.5rem;}

.parallaxtoph1{text-align:center;color:white!important;font-size:4rem;}
.gladiators{max-height:420px;}
  .gladiators > img{transition:all 0.2s ease;margin:auto;}
  .gladiators > img:hover{transform:scale(1.1);}
.whitelist{text-align:center;}
.parallaxtop{}
@media screen and (max-width:600px) {
  .gladiators > img{margin:auto;max-height:256px;}
  .row{flex-flow:column;}
.parallaxtop{transition:all 0.2s ease;margin:auto; width: 100%; height: 200px;}
.parallaxtoph1{text-align:center!important;margin:auto;color:white!important;font-size:3rem!important;}

}.hasEffect {
  cursor: pointer;
}
</style>

