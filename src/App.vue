<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent 
    :languagesList="languagesList" 
    :linksList="linksList"
    :HeaderSocials="HeaderSocials"
    />
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
  data() {
    return {
      // Header data
      languagesList: ["English", "Italian", "Spanish"],
      linksList: ["Home", "Pages", "Course Formats", "Courses", "Demos"],
      HeaderSocials: ["fa-facebook","fa-twitter","fa-instagram","fa-linkedin","fa-google-plus","fa-youtube"]
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/style/style.scss';


</style>
