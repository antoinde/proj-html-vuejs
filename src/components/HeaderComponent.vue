<template>
    <header>
        <div class="default-container">
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
                    <span class="socials">
                        <i v-for="(social, index) in HeaderSocials" :key="index" class="fa-brands" :class="social"></i>
                    </span>
                </div>
            </div>
        </div>

        <div class="separator"></div>

        <div class="default-container">
            <div class="bottom">
                <div class="logo-container">
                    <img class="mslogo" src="@/assets/img/footer-logo2x-50x56.png" alt="Master Study logo">
                </div>
                <div class="logo-text">
                    <strong>MASTER</strong> STUDY
                </div>
                <span class="category">
                    <i class="fa-solid fa-bars"></i>
                    <select name="category" id="category">
                        <option value="">CATEGORY</option>
                        <option value="">Business</option>
                        <option value="">Design</option>
                        <option value="">Development</option>
                        <option value="">Lifestyle</option>
                        <option value="">Office Productivity</option>
                        <option value="">IT & Software</option>
                        <option value="">Marketing</option>
                        <option value="">Art & Craft</option>
                        <option value="">Google</option>
                        <option value="">Food & Beverage</option>
                    </select>
                </span>
                <div class="searchBar"></div>
                <div class="forUsers"></div>
                <div class="profile-area"></div>
                <button class="addToPrefers"></button>
            </div>
        </div>
    </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
  props: {
    languagesList: Array,
    linksList: Array,
    HeaderSocials: Array
  }
}
</script>

<style lang="scss" scoped>
.top {
    display: flex;
    justify-content: space-between;
    padding: 5px 15px;
    margin-bottom: 5px;
    font-size: 0.90rem;
    color: grey;
    a{
        text-decoration: none;
        color: grey;
    }
    a:active{
        color: black;
    }
    select {
        border: none;
        color: grey;
    }
    .right{
        a,i{
            margin: 0 5px;
        }
        i:hover {
            color: darkgrey;
        }
        i:active {
            color: black;
        }
    }
    .socials {
        margin-left: 10px;
    }
}
.bottom {
    display: flex;
    align-items: center;
    padding: 15px;
    border: 1px solid black;
    column-gap: 10px;

    .logo-text{
        font-size: 1.8rem;

        strong {
            color: var(--azure-color);
        }
    }
    .category{
        display: flex;
        align-items: center;
        border-radius: 10px;
        padding: 0 10px;
        text-align: center;
        color: rgb(105, 105, 105);
        i{
            transform: translateX(20px);
        }
        
    }
    select {
        border: none;
        border-radius: 5px;
        width: auto;
        appearance: none;
        padding-left: 25px;
        padding-top: 3px;
        padding-bottom: 3px;
        color: rgb(105, 105, 105);
    }
    
}
.mslogo{
    background-color: var(--coralRed-color);
}

</style>