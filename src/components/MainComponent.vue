<template>
    <main>
      <AffiliateComponent />
      <PopularCoursesComponent
      :Cards="Cards"
      />
      <LearningInviteComponent />
    </main>
</template>

<script>
import AffiliateComponent from "./AffiliateComponent.vue";
import PopularCoursesComponent from "./PopularCoursesComponent.vue";
import LearningInviteComponent from "./LearningInviteComponent.vue";

export default {
    name: "MainComponent",
    components: { AffiliateComponent, PopularCoursesComponent, LearningInviteComponent },
    props: {
      Cards: Array
    }
}
</script>

<style lang="scss" scoped>


</style>