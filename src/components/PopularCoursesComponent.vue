<template>
    <section>
       <div class="default-container">
        <h4>Popular Development Courses</h4>
        <CardsComponent />            
       </div>
    </section>
</template>

<script>
import CardsComponent from './CardsComponent.vue';


export default {
    name: "PopularCoursesComponent",
    components: { CardsComponent },
    props: {
        Cards: Array
    }
}
</script>

<style lang="scss" scoped>
section{
    padding: 50px 0px;
}

</style>