<template>
    <main>
      <AffiliateComponent />
      <PopularDevCoursesComponent />
      <LearningInviteComponent />
      <RecentCoursesComponent />
      <PopularCoursesComponent />
      <InstructorOrBusinessComponent />
      <TestimonialComponent />
      <LateralTools />

    </main>
</template>

<script>
import AffiliateComponent from "./AffiliateComponent.vue";
import PopularDevCoursesComponent from "./PopularDevCoursesComponent.vue"
import LearningInviteComponent from "./LearningInviteComponent.vue";
import RecentCoursesComponent from "./RecentCoursesComponent.vue";
import PopularCoursesComponent from "./PopularCoursesComponent.vue";
import InstructorOrBusinessComponent from "./InstructorOrBusinessComponent.vue";
import TestimonialComponent from "./TestimonialComponent.vue";
import LateralTools from "./LateralTools.vue";

export default {
    name: "MainComponent",
    components: {
    AffiliateComponent,
    PopularDevCoursesComponent,
    LearningInviteComponent,
    RecentCoursesComponent,
    PopularCoursesComponent,
    InstructorOrBusinessComponent,
    TestimonialComponent,
    LateralTools
},
    props: {
      Cards: Array
    }
}
</script>

<style lang="scss" scoped>


</style>