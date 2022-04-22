<template>
  <div class="full-wrapper">
<div class="hero" style="min-height:50vh;width:100vw;background-color:#1e110d;display:flex;flex-flow:column;background-attachment:fixed;justify-content:center;background-blend-mode:soft-light;background-image:url(https://jooinn.com/images/dirt-texture-43.jpg);">
  <div class="hero-centered" style="margin:auto;text-align:center;">
   <h1 style="font-size:7rem;">Tomato Verse</h1>
   <br>
   <p>He who controls the Sauce Controls the TomatoVerse</p>
   <br>
   <h3>COMING SOON...</h3>
  </div>
</div>


<div class="row-wrapper" style="background-color:#ccc;padding:2rem;">
  <div class="row" style="display:flex;flex-flow:row;justify-content:center;">
  
    <div class="charbox" style="margin:0rem 1rem;">
      <img src="~/@/assets/tomato/Final2.png" style="width:400px;max-width:100%" alt="">
      <div class="desc" style="text-shadow:unset!important;color:black;">
      <br>
  <h3 style="text-shadow:unset!important;">Beefstake Bros</h3>
  <br>
<div class="row" style="justify-content:space-between;">
  <div class="chartitle">  
  <p>Total Population</p>
  <p>Trooper Population</p>
  <p>Faction Power</p>
  <p>Faction Prosperity</p>
</div>
  <div class="charval">
  <p>1500</p>
  <p>0</p>
  <p>0</p>
  <p>0</p></div>
</div>

      </div>
    </div>
    
    <div class="charbox" style="margin:0rem 1rem;">
      <img src="~/@/assets/tomato/Final1.png" style="width:400px;max-width:100%" alt="">
      <div class="desc" style="text-shadow:unset!important;color:black;">
      <br>
  <h3 style="text-shadow:unset!important;" >Cherry Cuties</h3>
  <br>
<div class="row" style="justify-content:space-between;">
  <div class="chartitle">
  <p>Total Population</p>
  <p>Trooper Population</p>
  <p>Faction Power</p>
  <p>Faction Prosperity</p></div>
  <div class="charval">
  <p>1500</p>
  <p>0</p>
  <p>0</p>
  <p>0</p></div>
</div>

      </div>
    </div>
    
    <div class="charbox" style="margin:0rem 1rem;">
      <img src="~/@/assets/tomato/Final3.png" style="width:400px;max-width:100%" alt="">
      <div class="desc" style="text-shadow:unset!important;color:black;">
      <br>
  <h3 style="text-shadow:unset!important;">Heirloom Hunks</h3>
  <br>
<div class="row" style="justify-content:space-between;">
  <div class="chartitle">
  <p>Total Population</p>
  <p>Trooper Population</p>
  <p>Faction Power</p>
  <p>Faction Prosperity</p></div>
  <div class="charval">
  <p>1500</p>
  <p>0</p>
  <p>0</p>
  <p>0</p></div>
</div>

      </div>
    </div>
  </div>

</div>


<div class="descwrap" style="padding:2rem;">
<div class="desctitle" style="width:1080px;margin:auto;"><br><br> <h1 style=" text-align:center;font-size:5rem;color:red;">Welcome To The Tomatoverse </h1><br><br>
<p style="color:black;">The TomatoVerse is a competitive community NFT game on the Ethereum blockchain. </p><br>
<p style="color:black;">Each Tomato NFT will grant access to one of three factions. The three factions will compete against each other in battles, with the winning faction being rewarded with the most Sauce NFTs. Tomato holders will be able to use these Sauce NFTs in a variety of ways to benefit themselves or their faction. </p>
<br><p style="color:black;">There are no rules in the TomatoVerse, and therefore factions will need to cooperate and self-organize to become the greatest faction.</p>
<br><p>The goal is to use sustainable NFT inflation mechanics to allow for a unique NFT experience. 
</p>

</div>
</div>



<div class="row-wrapper" style="background-color:#ccc;padding:2rem;">
<br><br> <h3 style=" text-align:center;font-size:3rem;color:white;">The TomatoVerse NFT Ecosystem </h3><br><br><br>
  <div class="row" style="display:flex;flex-flow:row;justify-content:center;">
  
    <div class="charbox" style="margin:0rem 1rem;">
      <img src="~/@/assets/tomato/Final2.png" style="width:400px;max-width:100%" alt="">
      <div class="desc" style="text-shadow:unset!important;color:black;">
      <br>
  <h3 style="text-shadow:unset!important;">Tomato Villagers</h3>
  <br>
  <ul>
  <li>Grants membership to factions</li>
  <li>Eligible for faction battle Sauce rewards
</li>
  <li>Max 4500 supply
</li></ul>

      </div>
    </div>
    
    <div class="charbox" style="margin:0rem 1rem;">
      <img src="~/@/assets/tomato/Final1.png" style="width:400px;max-width:100%" alt="">
      <div class="desc" style="text-shadow:unset!important;color:black;">
      <br>
  <h3 style="text-shadow:unset!important;" >Tomato Troopers</h3>
  <br>
  <ul>
  <li>Grants membership to factions</li>
  <li>Grants the ability to participate in PvP duels

</li>
  <li>Can be minted using Sauce NFTs + a Villager

</li></ul>

      </div>
    </div>
    
    <div class="charbox" style="margin:0rem 1rem;">
      <img src="~/@/assets/tomato/Final3.png" style="width:400px;max-width:100%" alt="">
      <div class="desc" style="text-shadow:unset!important;color:black;">
      <br>
  <h3 style="text-shadow:unset!important;">The Sauce</h3>
  <br>
  <ul>
  <li>Only obtained via winning faction battles
</li>
  <li>Burned upon use 

</li>
  <li>Can be used to mint Troopers, level a Trooper, or improve the prosperity of a faction

</li></ul>

      </div>
    </div>
  </div>

</div>



    </div>
</template>

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

