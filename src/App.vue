<template>
  <div id="app">
    <!-- HEADER -->
    <HeaderComponent 
    :languagesList="languagesList" 
    :linksList="linksList"
    :HeaderSocials="HeaderSocials"
    />
    <!-- MAIN -->
    <MainComponent :Cards="Cards"/>
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
      },
      Cards: [
          {
            genre: 'Development',
            path_img: '@/assets/img/895786_7b4b_2-544x322.jpg',
            title: 'The Complete iOs 10 & Swift 3 Developer Course',
            full_star: 4,
            half_star: 1,
            old_price: 199.99,
            new_price: 100
          },
          //    <i class="fa-solid fa-star"></i>
          //    <i class="fa-solid fa-star-half-stroke"></i>
          //    <i class="fa-regular fa-star"></i>
          {
            genre: 'Development',
            path_img: '@/assets/img/246154_d8b0_3-544x322.jpg',
            title: 'Web Design for Beginners: Real World Coding in HTML & CSS',
            full_star: 4,
            half_star: 1,
            old_price: 129.99,
            new_price: 65
          },
          {
            genre: 'Development',
            path_img: '@/assets/img/752950_b773-544x322.jpg',
            title: 'GitHub Ultimate: Master Git and GitHub - Beginner to Expert',
            full_star: 4,
            half_star: 1,
            old_price: 99.99,
            new_price: 50
          },
          {
            genre: 'Development',
            path_img: '@/assets/img/1253188_58f7_2-544x322.jpg',
            title: 'The Complete iOS 11 & Swift Developer Course - Build 20 Apps',
            full_star: 4,
            half_star: 1,
            old_price: 199.99,
            new_price: 100
          },
          {
            genre: 'Development',
            path_img: '@/assets/img/919872_ed54_6-544x322.jpg',
            title: 'Android Java Masterclass - Become an App Developer',
            full_star: 4,
            half_star: 1,
            old_price: 99.99,
            new_price: 50
          },
          {
            genre: 'Development',
            path_img: '@/assets/img/951684_9c1a_2-544x322.jpg',
            title: 'Xamarin Forms: Build Native Cross-platform Apps with C#',
            full_star: 4,
            half_star: 1,
            old_price: 189.99,
            new_price: 95
          },
          {
            genre: 'Design',
            path_img: '@/assets/img/1561458_7f3b-544x322.jpg',
            title: 'CSS - The Complete Guide 2020 (incl. Flexbox, Grid & Sass)',
            full_star: 5,
            half_star: '',
            old_price: 199.99,
            new_price: 100
          },
          {
            genre: 'Design',
            path_img: '@/assets/img/1208228_d61c_4-544x322.jpg',
            title: 'Digitally Painting Light and Color: Amateur to Master',
            full_star: 4,
            half_star: 1,
            old_price: 139.99,
            new_price: 70
          },
          {
            genre: 'Art & Crafts',
            path_img: '@/assets/img/186792_41e4_4-544x322.jpg',
            title: 'Become an Arabic Calligraphy Artist from Scratch',
            full_star: 4,
            half_star: 1,
            old_price: '',
            new_price: 199.99
          },
          {
            genre: 'Google',
            path_img: '@/assets/img/1776542_30b1-544x322.jpg',
            title: 'Google Searching Ninja!',
            full_star: 3,
            half_star: 1,
            old_price: 89.99,
            new_price: 45
          },
          {
            genre: 'Arts & Crafts',
            path_img: '@/assets/img/949316_2a64_11-544x322.jpg',
            title: 'Foundations for Mastering Watercolor Painting',
            full_star: 4,
            half_star: 1,
            old_price: 19.99,
            new_price: 10
          },
          {
            genre: 'Food & Beverage',
            path_img: '@/assets/img/366802_6fcc-544x322.jpg',
            title: 'Get Wine-Smart',
            full_star: 4,
            half_star: 1,
            old_price: 49.99,
            new_price: 25
          },
          {
            genre: 'Arts & Crafts',
            path_img: '@/assets/img/381588_2e6d_4-544x322.jpg',
            title: 'The Colored Pencil Drawing Course',
            full_star: 4,
            half_star: '',
            old_price: 34.99,
            new_price: 18
          },
          {
            genre: 'Arts & Crafts',
            path_img: '@/assets/img/838056_611a_3-544x322.jpg',
            title: 'Paint Realistic Watercolor and Botanicals - STUDIO BASICS',
            full_star: 4,
            half_star: '',
            old_price: 69.99,
            new_price: 35
          },
          {
            genre: 'Arts & Crafts',
            path_img: '@/assets/img/1414956_d944_15-544x322.jpg',
            title: 'Mastering Brushstrokes - Part 1',
            full_star: 5,
            half_star: '',
            old_price: 19.99,
            new_price: 10
          },
          {
            genre: 'Arts & Craft',
            path_img: '@/assets/img/1109398_4c13-544x322.jpg',
            title: 'Paint Realistic Watercolour and Botanicals - MAGNOLIAS',
            full_star: 5,
            half_star: '',
            old_price: 69.99,
            new_price: 35
          }
        ]
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/style/style.scss';


</style>
