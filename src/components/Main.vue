<template>
  <!-- since main is going to be very large its going to devided in many different components -->
  <div>
    <!-- BUILD YOUR TEAM -->
    <BuildYourTeam />
    <!-- ConstructCareer -->
    <ConstructCareer />
    <!-- Section with obtainded results -->
    <ResultsObtained />
    <!-- Latest courses -->
    <LatestCourses />
  </div>
</template>

<script>
import BuildYourTeam from './BuildYourTeam'
import ConstructCareer from './ConstructCareer'
import ResultsObtained from './ResultsObtained'
import LatestCourses from './LatestCourses.vue'
export default {
    components:{
        BuildYourTeam,
        ConstructCareer,
        ResultsObtained,
        LatestCourses
    }
}
</script>

<style>

</style>