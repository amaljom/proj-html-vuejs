<template>
    <div class="bg-result-container">
      <div class="card-contenitore d-flex justify-content-around py-5 align-items-center text-center">
          <div v-for="(element, index) in results" :key="index">
            <h2> {{ element.number}} </h2>
            <span> {{ element.text }} </span>  
          </div>
      </div>
    </div>
</template>

<script>
export default {
    data:function () {
        return{
            results:[
              {
                number:1.926,
                text:'FINISHED LESSONS'
              },
              {
                number:3.092,
                text:'ENROLLED LEARNERS'
              },
              {
                number:200,
                text:'FINISHED LESSONS'
              },
              {
                number:'100%',
                text:'FINISHED LESSONS'
              }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import"../assets/style/Variable.scss";
.bg-result-container{
  background-color: #faf8f6;
}
div h2{
  color: #20ad96;
  font-weight: bolder;
  font-size: 4rem;
}
span{
  font-weight: bolder;
  color: black;
}
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
}
</style>