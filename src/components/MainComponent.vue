<template>
    <main>
      <AffiliateComponent />
      <PopularCoursesComponent
      :Cards="Cards"
      />
      <LearningInviteComponent />
      <RecentCoursesComponent />
      <PopularCoursesComponent />

    </main>
</template>

<script>
import AffiliateComponent from "./AffiliateComponent.vue";
import PopularCoursesComponent from "./PopularCoursesComponent.vue";
import LearningInviteComponent from "./LearningInviteComponent.vue";
import RecentCoursesComponent from "./RecentCoursesComponent.vue";

export default {
    name: "MainComponent",
    components: { AffiliateComponent, PopularCoursesComponent, LearningInviteComponent, RecentCoursesComponent },
    props: {
      Cards: Array
    }
}
</script>

<style lang="scss" scoped>


</style>