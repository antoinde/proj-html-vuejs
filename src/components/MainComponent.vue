<template>
    <main>
      <AffiliateComponent />
      <PopularDevCoursesComponent />
      <LearningInviteComponent />
      <RecentCoursesComponent />
      <PopularCoursesComponent />
      <InstructorOrBusinessComponent />

    </main>
</template>

<script>
import AffiliateComponent from "./AffiliateComponent.vue";
import PopularDevCoursesComponent from "./PopularDevCoursesComponent.vue"
import PopularCoursesComponent from "./PopularCoursesComponent.vue";
import LearningInviteComponent from "./LearningInviteComponent.vue";
import RecentCoursesComponent from "./RecentCoursesComponent.vue";

export default {
    name: "MainComponent",
    components: { 
      AffiliateComponent,
      PopularDevCoursesComponent,
      LearningInviteComponent, 
      RecentCoursesComponent, 
      PopularCoursesComponent, 
    },
    props: {
      Cards: Array
    }
}
</script>

<style lang="scss" scoped>


</style>