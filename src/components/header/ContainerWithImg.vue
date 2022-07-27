<template>
  <div class="d-flex justify-content-between mt-5 py-3 background-container">
    <div class="container-size">
        <!-- titolo -->
        <h1>Complete Your Dreams In Javas Programming</h1>
        <!-- scritta -->
        <p>
            Learn any coding program in distance and for a reasonable fee.
            You don't gabe to struggle alone, you've got out assitance and help.
        </p>
        <!-- Bottone -->
        <div class="d-flex text-white button">
            <i class="fa-solid fa-download pe-3"></i>
            <span>Download Free E-book</span>
        </div>
    </div>
    <div> <img src="../../assets/img/home-5-hero-image.png" alt=""> </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
img{
    width: 540px;
}
h1{
    color: #3f3a64;
    font-size: 4rem;
    font-weight: bolder;
}
p{
   color: #b4b1be;
   font-weight: bolder;
   font-size: 20px;
}
.container-size{
    width: 35%;
}
.button{
    padding: 18px 19px;
    background-color: #20ad96;
    border-radius: 12px;
    width: 52%;
    transition: .2s;
     &:hover{
        background-color: #3f3a64;
        cursor: pointer;
     }
}

</style>