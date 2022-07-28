<template>
  <div class="card-contenitore d-flex justify-content-around my-5 py-3 background-container">
        <div class="container-size">
            <!-- prima del titolo -->
            <span class="color-special">WHY ESITATE TO REGISTER?</span>
            <!-- titolo -->
            <div class="d-flex">
                <h1>Learn At Your Own&nbsp;<span class="thinner">Pace</span></h1>
            </div>
            <div>
                <ul>
                    <li class="pb-3" v-for="(benefit, index) in benefits" :key="index"><i class="fa-solid fa-check pe-2"></i> {{ benefit.text}}</li>
                </ul>
            </div>
            <ButtonComponent 
                :url="url"
                :buttonText="buttonTxt" />
        </div>
        <div class="img-container-background position-relative">
             <img src="../../assets/img/home-5-image-01.png" alt=""> 
             <img class="decoration" src="../../assets/img/maxcoach-shape-05.png" alt="">
        </div>
    </div>
</template>

<script>
import ButtonComponent from './ButtonComponent'
export default {
    components:{
        ButtonComponent
    },
    data:function(){
        return{
            // BUTTON
            buttonTxt:"Get started for free",
            url:'#'
        }
    },
    props:['benefits']

}
    

</script>

<style lang="scss" scoped>
@import"../../assets/style/Variable.scss";
.color-special{
    color:$ElementOverTitles;
}
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
}

h1{
    color: $SectionsTitleColor;
    font-size: 3rem;
    font-weight: bolder;
}
.thinner{
    font-size: 3rem;
    color: $SectionsTitleColorSecondary;
    font-weight: 200;
}

.container-size{
    width: 33%;
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
img{
    width: 500px;
    position: relative;
    left: 76px;
}
.decoration{
    width: 200px;
    position: absolute;
    left: 480px;
    bottom: 50px;
}
.img-container-background{
    background-image: url(../../assets/img/underlay-shape-grey.svg);
    background-repeat: no-repeat;
    background-size: 450px;
    background-position-y: bottom;
    background-position-x: left;
    width: 597px;
}
ul li{
    list-style: none;
}
ul{
    padding-left: 0;
}
ul li i{
    color: #20ad96;
}
.star-now-button{
    width: 60%;
}
</style>