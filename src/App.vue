<template>
  <HeaderComponent/>
  <MainComponent/>
  <BuyComics/>
  <FooterComponent/>
</template>

<script>
import MainComponent from './components/MainComponent.vue'
import BuyComics from './components/BuyComics.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import FooterComponent from './components/FooterComponent.vue'
  export default {
    components:{
      HeaderComponent,
      MainComponent,
      BuyComics,
      FooterComponent,

    }
  }
</script>

<style scoped>

</style>

