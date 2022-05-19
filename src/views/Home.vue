<template>
  <div class="full-wrapper" style="">

  <div class="hero" style="overflow:hidden;
    backdrop-filter: blur(7px);height:100vh;width:100vw;z-index:50;display:flex;flex-flow:column;justify-content:center;">     
  
  <img src="~/@/assets/tomato/tomato.png" style="
    height:100%;width:auto;
   z-index:10;margin:0rem  auto;
    max-height:23vh;
    image-rendering: -webkit-optimize-contrast;" alt="">
 
  <img src="~/@/assets/tomato/verse.png" style="
    height:100%;width:auto;
   z-index:10;margin:0rem auto;max-height:20vh;
    image-rendering: -webkit-optimize-contrast;" alt="">
<!--
 <img src="~/@/assets/tomato/VINES.png" style="
    image-rendering: -webkit-optimize-contrast;width:100vh;margin:unset; transform:rotate(-90deg);transform=origin:bottom left; position: absolute;
    bottom: 29vh; 
    left: -21vw;image-rendering: -webkit-optimize-contrast;" alt="">-->
 </div> 

  <div class="background-scroller" style="position:fixed;bottom:0px;">
  <div class="tomatorow" style="height:100vh;width:400vw;overflow:visible;display:flex;flex-flow:row;opacity:0.5;">
    <div style="width:100vw;display:flex;flex-flow:wrap; justify-content:center;">
   


</div>
  
  </div>

  </div>

  <div class="mint-cta-box" style="display:flex;flex-flow:row;justify-content:space-between;padding:1rem;position:fixed;bottom:2rem; right:2rem;z-index:200;width:660px;height:80px;background:#b6b0e8;border-radius:0.25rem;box-shadow:4px 4px #efebe8;" >
  
  <div style="display:flex;flex-flow:row;">
  <a href="https://discord.gg/6Pnbwkk3tu"><img src="~/@/assets/discordwhite.svg" style="width:3rem;padding:0.25rem;height:3rem;" alt=""></a> 
  <div><p style="color:#efebe8;opacity:0.5;line-height:1;font-size:0.75rem;padding-left:1rem;padding-bottom:unset;margin-bottom:0.25rem;">JOIN OUR GROWING DISCORD</p>
  <p style="font-weight:bold;padding-left:1rem;margin:auto;color:#efebe8;line-height:1;font-size:1.5rem;">ENTER TOMATOVERSE</p></div>
  </div>
  
  <div class="buttoncta" style="">
  <b style="margin:auto;
    line-height: 1rem;">WHITEPAPER </b>
  <b style="margin:auto;
    line-height: 1rem;"><img class="arrow" src="~/@/assets/right-arrow.svg" style="width:16px;" alt=""></b>
  </div>

  </div>
    </div>
</template>
-
<script>
import { mapState, mapActions } from 'vuex';
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
    
  },
};
</script>
<style scoped>



@media screen and (max-width:600px) {

}
</style>

