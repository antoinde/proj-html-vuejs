<template>
    <header>
        <div class="top">
            <!-- ###### Selettore della lingua -->
            <div class="left">
                <select name="language" id="language">
                    <!-- lingue inserite dinamicamente -->
                    <option v-for="(lang, index) in languagesList" :key="index" :value="lang"> {{ lang }} </option>
                </select>
            </div>
            <!-- ###### Links e social -->
            <div class="right">
                <!-- links -->
                <span>
                    <a v-for="(link, index) in linksList" :key="index" href="#"> {{ link }} </a>
                </span>
                <!-- social network -->
                <span>
                    <i v-for="(social, index) in socials" :key="index" class="fa-brands" :class="social"></i>
                </span>
            </div>
        </div>
        <div class="separator"></div>
        <div class="bottom"></div>
    </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
  props: {
    languagesList: Array,
    linksList: Array,
    socials: Array
  }
}
</script>

<style lang="scss" scoped>
.top {
    display: flex;
    justify-content: space-between;
}

</style>