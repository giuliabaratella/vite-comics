<template>
  <HeaderComponent/>
  <MainComponent/>
  <FooterComponent/>
</template>

<script>
import MainComponent from './components/MainComponent.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import FooterComponent from './components/FooterComponent.vue'
  export default {
    components:{
      HeaderComponent,
      MainComponent,
      FooterComponent,

    }
  }
</script>

<style scoped>

</style>

