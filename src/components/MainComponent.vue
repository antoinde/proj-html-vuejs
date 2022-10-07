<template>
    <main>
      <section>
        <nav>
          <div class="container">
            <a>
              <span class="icon"> <i class="fa-solid fa-chart-column"></i> </span>
              <span class="text"> Business </span>
            </a>
            <a>
              <span class="icon"> <i class="fa-solid fa-palette"></i> </span>
              <span class="text"> Design </span>
            </a>
            <a>
              <span class="icon"> <i class="fa-solid fa-gear"></i> </span>
              <span class="text"> Development </span>
            </a>
            <a>
              <span class="icon"> <i class="fa-regular fa-face-smile-beam"></i> </span>
              <span class="text"> Lifestyle </span>
            </a>
            <a>
              <span class="icon"> <i class="fa-solid fa-print"></i> </span>
              <span class="text"> Office Productivity </span>
            </a>
          </div>
        </nav>
        <div class="images_area">
          <div class="split50 left">
            <div class="colored_area"></div>
          </div>
          <div class="split50 right">
            <img src="@/assets/img/slide-1.jpg" alt="Affiliate guys">
            <div class="color_trick"></div>
          </div>
          
        </div>
      </section>
    </main>
</template>

<script>
export default {
  name: 'MainComponent',
}
</script>

<style lang="scss" scoped>
nav {
  background-color: var(--footer-nav-color);
  margin-bottom: 20px;
}
.container{
  display: flex;
  column-gap: 45px;
  justify-content: center;
  padding: 15px;
  .icon i{
    color: #fff;
    margin-right: 5px;
  }
  .text {
    color: #fff;
  }
}
.images_area{
  display: flex;
  .split50{
    width: 50%;
    height: 300px;
  }
  img{
    height: 300px;
  }
  .left{
    display: flex;
    justify-content: flex-end;
    .colored_area{
      background-color: var(--coralRed-color);
      height: 300px;
      width: 740px;
      position: relative;

    }
  }
  .right{
    position: relative;
    overflow: hidden;
    .color_trick{
      background-color: var(--coralRed-color);
      height: 300px;
      width: 740px;
      transform: translateY(-551px);
      rotate: 70deg;
      position: absolute;
      left: -950px;
    }
  }
}
</style>