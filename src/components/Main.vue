<template>
  <!-- since main is going to be very large its going to devided in many different components -->
  <div>
    <!-- BUILD YOUR TEAM -->
    <BuildYourTeam />
    <!-- ConstructCareer -->
    <ConstructCareer />
  </div>
</template>

<script>
import BuildYourTeam from './BuildYourTeam'
import ConstructCareer from './ConstructCareer'
export default {
    components:{
        BuildYourTeam,
        ConstructCareer
    }
}
</script>

<style>

</style>