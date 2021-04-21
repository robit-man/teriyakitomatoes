<template>
  <div class="block">
 
    <div class="logo-center-wrapper" style="">
      <vh-copy class="copy-button"
      :data="'0x5D2C6545d16e3f927a25b4567E39e2cf5076BeF4'"
      :label="'Contract'"
      :confirm_dialog="'buefy'"
      @copied="copiedData">
      <img class="copy-icon" src="~/@/assets/favicon.png" width="48px" height="48px" style="" alt="$KAPPA">
      </vh-copy> <vh-copy class="sale-button"
      :data="'0x0d3dce906c833291d1935579e0289a1afd2943d1'"
      :label="'Sale'"
      :confirm_dialog="'buefy'"
      @copied="copiedData">
      <img class="copy-icon" src="~/@/assets/wallet.png" width="48px" height="48px" style="" alt="$KAPPA">
      </vh-copy>
      <jj-parallax-card class="mt-6 para-mobile" lightColor="transparent" style="margin:auto;float:left; width: 300px; height: 280px;" @click="click">
      <div slot="front">
      <img src="~/@/assets/KAPPA.svg" width="512px;" class="mt-4" alt="">
      </div>
</jj-parallax-card>
      <jj-parallax-card class="mt-6 para-desktop" lightColor="transparent" style="margin:auto;float:left; width: 512px; height: 490px;" @click="click">
      <div slot="front">
      <img src="~/@/assets/KAPPA.svg" width="512px;" class="mt-4" alt="">
      </div>
</jj-parallax-card>
      <div class="logo-title"><h1 style="">$KAPPA</h1></div>

    </div>
    <div class="data-wrapper" style="">
      <div class="data-title" style="">ACCESS THE CONTRACT </div>
      <div class="data-hexagons"  style="">
      <a class="hexagon-module" target="_blank" href="https://www.dextools.io/app/uniswap/pair-explorer/0xefa2e1e46b83d572d01521c4c64845b0227b6314">
          <img width="64px" height="64px" src="~/@/assets/dextools.png" alt="">
          </a>
       <a class="hexagon-module" target="_blank" href="https://app.uniswap.org/#/swap">
          <img width="64px" height="64px" src="~/@/assets/uniswap.png" alt="">
        </a>
        <a class="hexagon-module" target="_blank" href="https://etherscan.io/address/0x5d2c6545d16e3f927a25b4567e39e2cf5076bef4">
          <img width="64px" height="64px" src="~/@/assets/etherscan.png" alt="">
        </a>
        <a class="hexagon-module" target="_blank" href="https://app.uniswap.org/#/add/0x5D2C6545d16e3f927a25b4567E39e2cf5076BeF4/ETH">
          <img width="64px" height="64px" src="~/@/assets/liquidity.png" alt="">
       </a>
        </div>
    </div>

  </div>
</template>

<script>
import { mapState, mapActions } from 'vuex';
import JJParallaxCard from 'jj-parallax-card'

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
  computed: {
    ...mapState(['settings']),
    isValid() {
      return parseFloat(this.form.quantity);
    },
    maxStrike() {
      const exchangeRate = this.settings.exchangeRates[this.form.asset];
      return exchangeRate && exchangeRate.usd ? exchangeRate.usd : 1e9;
    }
  },
  methods: {
    
    ...mapActions(['SendDai']),
    handleSubmit() {
      this.SendDai({
        //address: '0xb72027693a5B717B9e28Ea5E12eC59b67c944Df7',
        value: this.form.quantity
      });
    },
    maxStake() {
      this.form.quantity = this.$store.state.settings.balance;
    }
  },components: {
    'jj-parallax-card':JJParallaxCard,
  },
};
</script>
<style scoped>
.hasEffect {
  cursor: pointer;
}
</style>

