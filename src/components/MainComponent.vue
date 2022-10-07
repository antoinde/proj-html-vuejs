<template>
    <main>
      <AffiliateComponent />
      <PopularCoursesComponent
      :Cards="Cards"
      />
    </main>
</template>

<script>
import AffiliateComponent from "./AffiliateComponent.vue";
import PopularCoursesComponent from "./PopularCoursesComponent.vue";

export default {
    name: "MainComponent",
    components: { AffiliateComponent, PopularCoursesComponent },
    props: {
      Cards: Array
    }
}
</script>

<style lang="scss" scoped>


</style>