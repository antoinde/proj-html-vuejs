<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent />
    <!-- MAIN -->
    <MainComponent />
    <!-- FOOTER -->
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent
  },
}
</script>

<style lang="scss">
@import '@/assets/style/style.scss';


</style>
