<template>
    <div style="height:100vh;margin:unset;overflow:hidden;">
      
      <div class="menu">
      <div class="row" style="max-width:112rem;margin:auto;width:100%;justify-content:space-between;">
        <a href="/"> <div class="tomatobutton">TOMATOVERSE</div></a>

        <div class="linkrow">

        <a href="" class="menubutton soon" style="border:1px solid #1115;">
          MINT
        </a>
        <a href="" class="menubutton soon">
          DUELS
        </a>
        <a href="" class="menubutton soon">
          TROOPERS
        </a>
        <a href="" class="menubutton soon">
          WHITEPAPER
        </a>
        <a href="" class="menubutton soon">
          OPENSEA
        </a>
        <a target="_blank" href="https://discord.gg/6Pnbwkk3tu" class="menubutton nobg ">
          <img src="~/@/assets/discordmenu.svg" style="width:2rem;padding:0.25rem;height:3rem;" alt="">
        </a>
        <a target="_blank" href="https://twitter.com/TomatoVerse" class="menubutton nobg ">
          <img src="~/@/assets/twittermenu.svg" style="width:2rem;padding:0.25rem;height:3rem;" alt="">
        </a>
        
        </div>
        </div>
      </div>

    <div id="app" class="" style="">
      <VueLoadingIndicator v-if="settings.loading" class="overlay big" />
      <div v-else>
        <router-view :key="$route.path" />
      </div>
    </div>
  </div>
</template>

<script>
import { mapState, mapActions } from 'vuex';

export default {
  computed: {
    ...mapState(['settings'])
  },
  methods: {
    ...mapActions(['init'])
  },
  async created() {
    this.init();
  }
};
</script>
