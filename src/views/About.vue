<template>
  <div class="full-wrapper">
    
  
      <div class="about-wrap">
         <vh-copy class="para-desktop copy-button"
      :data="'0x5D2C6545d16e3f927a25b4567E39e2cf5076BeF4'"
      :confirm_dialog="'buefy'"
      @copied="copiedData">
      Contract Address
</vh-copy><br>
 <h1></h1>
<br><p>

</p>    <br>    <router-link :to="{ name: 'home' }" >
     <img src="~/@/assets/kappa-36.png" style="height:64px;filter:invert(1);" alt="">
    </router-link></div>

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
.hasEffect {
  cursor: pointer;
}
</style>

