<script>
//1- Importazione del componenente necessario che voglio aggiungere qua

import AppHeader from './components/AppHaeder.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppAdsNavbar from './components/AppAdsNavbar.vue';
export default {
  data() {
    return {

    }
  },
  //2- Dichiarazione del componente 
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppAdsNavbar,
  },
  methods: {

  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppAdsNavbar />
  <AppFooter />
</template>

<style scoped>
.container {
  max-width: 1300px;
  margin: 0 auto;
  position: relative;
}

</style>
