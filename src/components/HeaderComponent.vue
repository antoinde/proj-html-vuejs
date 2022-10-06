<template>
    <header>
        
        <div class="default-container"> <!-- top -->
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
        
        <div class="separator"></div> <!-- separator -->
        
        <div class="default-container"> <!-- bottom -->
            <div class="bottom">
                <div class="logo-container">
                    <img class="img_mslogo" src="@/assets/img/header-logo2x-50x56.png" alt="Master Study logo">
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
                <div class="searchBar">
                    <input type="text" placeholder="Search courses">
                    <button><i class="fa-solid fa-magnifying-glass"></i></button>
                </div>
                <div class="forUsers">
                    <a href="#">
                        <i class="fa-solid fa-bullhorn"></i>
                        <span> Become an Instructor</span>
                    </a>
                    <a href="#">
                        <i class="fa-solid fa-briefcase"></i>
                        <span> For Enterprise</span>
                    </a>
                </div>
                <div class="profile-area">
                    <a>
                        <i class="fa-regular fa-user"></i>
                        <span> Log in</span>
                    </a>
                    <a class="typeButtonRose" href="#">SIGN UP</a>
                    <button class="addToPrefers">
                        <i class="fa-regular fa-bookmark"></i>
                    </button>
                </div>
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
    position: relative;
    display: flex;
    align-items: center;
    padding: 5px;
    font-size: 0.8rem;

    .logo-text{
        font-size: 1.8rem;
        margin-left: 5px;

        strong {
            color: var(--azure-color);
        }
    }
    .img_mslogo{
        background-color: var(--coralRed-color);
    }
    .category{
        display: flex;
        align-items: center;
        border-radius: 10px;
        padding: 0 10px;
        text-align: center;
        margin-left: -10px;
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
    
    .forUsers{
         margin: 0 20px;
         display: flex;
         column-gap: 15px;
    }
    .profile-area {
        position: absolute;
        right: 0;
        display: flex;
        align-items: center;
        column-gap: 15px;
    }
    button.addToPrefers{
        background-color: #fff;
        padding: 5px 10px;
        border: none;
        border-radius: 25px;
    }
    button.addToPrefers:hover{
        background-color: #e5e5e5;
    }
}

</style>