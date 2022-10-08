<template>
    <section>
        <div class="default-container">

            <div class="center-text">
                <h4>Popular courses</h4>
                <div>
                    <span>Discover our most popular courses for self learning</span>
                </div>
            </div>

            <PopularCardsComponent />

            <div class="center-text two">
                <span class="square"><i class="fa-solid fa-angle-left"></i></span>
                <span class="square"><i class="fa-solid fa-angle-right"></i></span>
            </div>

        </div>

    </section>
</template>

<script>
import PopularCardsComponent from './PopularCardsComponent.vue';


export default {
    name: "PopularCoursesComponent",
    components: { PopularCardsComponent }
}
</script>

<style lang="scss" scoped>
section {
    padding: 50px 0px;

    .center-text {
        text-align: center;
        margin-bottom: 40px;

        h4 {
            font-size: 2.2rem;
            margin-bottom: 10px;
            margin-top: 0px;
        }

        div {
            color: grey;

            span {
                margin: 0 10px;
                border-radius: 25px;
                padding: 10px;
            }
        }
    }
    .center-text.two{
        margin-top: 60px;
        margin-bottom: 20px;
        .square{
            padding: 10px 13px;
            border: 1px solid grey;
            background-color: #fff;
            cursor: pointer;
        }
        .square:hover{
            background-color: var(--search-button-color);
            color: #fff;
        }
    }
}
</style>