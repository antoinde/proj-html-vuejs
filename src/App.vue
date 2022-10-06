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
    <FooterComponent 
    :FooterCards="FooterCards"
    />
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
      HeaderSocials: ["fa-facebook","fa-twitter","fa-instagram","fa-linkedin","fa-google-plus","fa-youtube"],
      // Footer data
      FooterCards: {
        about:{
          title: 'ABOUT',
          text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eveniet voluptatem quasi inventore in quod commodi harum facilis aliquam ullam illum cum molestiae repudiandae debitis asperiores modi voluptatum odio, soluta quaerat.'
        },
        contact:{
          title: 'CONTACT',
          location: 'USA, California 20, First Avenue, California',
          telephone: 'Tel.:+1 212 458 300 32',
          fax: 'Fax.:+1 212 375 24 14',
          email: 'info@masterstudy.com'
        },
        FooterSocials: {
          title: 'SOCIAL NETWORK',
          socials: [
            "fa-facebook","fa-instagram","fa-linkedin","fa-pinterest","fa-twitter","fa-dribbble","fa-google-plus","fa-skype"
          ],
        }
        
        
      }
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/style/style.scss';


</style>
