<template>
    <div class="background pt-5">
        <div class="card-contenitore text-center">
            <h1>Start today for getting&nbsp;<span class="thinner">Online Certification</span></h1>
            <h1 class="Bigger-h1">You can be your own guiding star with our help</h1>
            <ButtonComponent 
                :url="UrlGetStarted"
                :buttonText="buttonTxt" />
            <div>
                <img class="decoration-1" src="../../assets/img/maxcoach-shape-01.png" alt="">
            </div>
            <div>
                <img class="decoration-2" src="../../assets/img/maxcoach-shape-02.png" alt="">
            </div>
            <div class="circle"></div>
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
        // data for button
        return{
            UrlGetStarted:'#',
            buttonTxt:'Get started now'
        }
    }
}
</script>

<style lang="scss" scoped>
@import"../../assets/style/Variable.scss";
.color-special{
    color:#696b86;
}
.background{
    background-color: #f3f3f3;
}
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
}
h1{
    color: $SectionsTitleColor;
    font-size: 1.8rem;
    font-weight: bolder;
}
.Bigger-h1{
    color: $SectionsTitleColor;
    font-size: 2.5rem;
    font-weight: bolder;
}
.thinner{
    font-size: 1.8rem;
    color: $SectionsTitleColorSecondary;
    font-weight: 200;
}
.star-now-button{
    padding: 10px;
    background-color: #20ad96;
    text-align: center;
    transition-duration: 0.3s;
    border-radius: 7px;
    width: 25%;
    margin: 0 auto;
    &:hover{
        background-color: #3f3a64;
    }
}
.star-now-button a{
    text-decoration: none;
    color: #ffffff;
    font-weight: bolder;
}
.decoration-1{
    position: relative;
    bottom: 65px;
    right: 38%;
}
.decoration-2{
    position: relative;
    bottom: 90px;
    left: 40%;
}
.circle{
    border: solid 4px #c3c3a7;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    position: relative;
    bottom: 300px;
    left: 36px;
}
</style>