<template>
    <footer>
        <div class="container top">
          <!-- Card (x3) -->
          <div v-for="(card, index) in FooterCards" :key="index" class="card">
            <h3>{{ card.title }}</h3>
            <p>{{ card.text }}</p>
            <p>{{ card.location }}</p>
            <p>{{ card.telephone }}</p>
            <p>{{ card.fax }}</p>
            <p class="email">{{ card.email }}</p>
            <div class="social-container">
              <i v-for="(social, index) in card.socials" :key="index" 
                class="fa-brands" :class="social" >
              </i>
            </div>
          </div>
          <!-- Card (image) -->
          <div class="card">
            <img src="@/assets/img/Top-udemy-courses-90-percent-off.jpg" alt="Udemy image Discount 80% off">
          </div>
          
        </div>

        <div class="separator"></div>

        <div class="container bottom">
          <img src="@/assets/img/footer-logo2x-50x56.png" alt="Footer MasterStudy logo">
          <span> Copyright &copy; 2022. <u>MasterStudy</u> Theme by <u>StylemixThemes</u> </span>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'FooterComponent',
  props:{
    FooterCards: Object
  }

}
</script>

<style lang="scss" scoped>
  footer{
    background-color: var(--footer-nav-color);
    color: #fff;
    font-size: 0.7rem;
  }
  .container.top {
    max-width: 1100px;
    margin: 0 auto;
    padding: 50px 0px;
    display: flex;
    flex-wrap: wrap;
    column-gap: 30px;
  }
  .card{
    width: calc(100% / 4 - 23px);
    p{
      line-height: 1.1rem;
    }
  }
  .email{
    color: grey;
    filter: opacity(0.5);
    &:hover{
      filter: opacity(1);
    }
  }
  .social-container{
    display: flex;
    flex-wrap: wrap;
    i{
      width: calc(100% / 4 - 10px);
      font-size: 2.3rem;
      margin: 5px;
    }
    
  }
  .separator{
    border-color: grey;
  }
  .container.bottom {
    max-width: 1100px;
    margin: 0 auto;
    padding: 20px 0px;
    display: flex;
    align-items: center;
    img{
      width: 30px;
      margin-right: 10px;
    }
  }
</style>