<template>
    <div style="height:100vh;margin:unset;overflow:hidden;">
      
      <div class="menu">
      <div class="row" style="max-width:112rem;margin:auto;width:100%;justify-content:space-between;">
        <a href="/"> <div class="tomatobutton">TOMATOVERSE</div></a>

        <div class="linkrow">

        <a href="" class="menubutton" style="border:1px solid #1115;">
          MINT
        </a>
        <a href="" class="menubutton">
          DUELS
        </a>
        <a href="" class="menubutton">
          TROOPERS
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
