<template>
    <main>
        <nav >
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
</style>