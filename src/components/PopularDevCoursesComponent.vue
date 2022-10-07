<template>
    <section>
        <div class="default-container">


            <h3>Popular development courses</h3>

            <PopularCardsDevComponent />


        </div>

    </section>
</template>

<script>
import PopularCardsDevComponent from './PopularCardsDevComponent.vue';


export default {
    name: "PopularDevCoursesComponent",
    components: {
        PopularCardsDevComponent 
    }
}
</script>

<style lang="scss" scoped>
section {
    padding: 50px 0px;
}
</style>