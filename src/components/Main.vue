<template>
  <!-- since main is going to be very large its going to devided in many different components -->
  <div>
    <!-- BUILD YOUR TEAM -->
    <BuildYourTeam />
    <!-- ConstructCareer -->
    <ConstructCareer />
    <!-- Section with obtainded results -->
    <ResultsObtained />
  </div>
</template>

<script>
import BuildYourTeam from './BuildYourTeam'
import ConstructCareer from './ConstructCareer'
import ResultsObtained from './ResultsObtained'
export default {
    components:{
        BuildYourTeam,
        ConstructCareer,
        ResultsObtained
    }
}
</script>

<style>

</style>