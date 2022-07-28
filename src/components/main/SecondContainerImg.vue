<template>
  <div class="card-contenitore d-flex justify-content-around my-5 py-3 background-container">
        <div class="img-container-background position-relative">
             <img src="../../assets/img/home-5-image-02.png" alt=""> 
             <img class="decoration" src="../../assets/img/maxcoach-shape-07.png" alt="">
             <img class="decoration2" src="../../assets/img/maxcoach-shape-01.png" alt="">
             <div class="circle"></div>
        </div>
        <div class="container-size">
            <!-- prima del titolo -->
            <span class="color-special">WHAT ARE YOU LOOKING FOR?</span>
            <!-- titolo -->
            <div class="d-flex">
                <h1>Learn on Your&nbsp;<span class="thinner">Mobile</span></h1>
            </div>
            <h1>Anytime!</h1>
            <div>
                <p>Save lessons for later and revise or write notes at anu time and on multiple devices on you way.
                    Never interfere with activities of enjoyment of other precious moments.
                </p>
            </div>
            <ButtonComponent 
                :url="url"
                :buttonText="buttonTxt" />
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
            buttonTxt:"Download our App",
            url:'#'
        }
    },
}
</script>

<style lang="scss" scoped>
@import"../../assets/style/Variable.scss";
.color-special{
    color:#696b86;
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
    width: 39%;
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
    width: 400px;
    position: relative;
    left: 76px;
    z-index: 200;
}
.decoration{
    width: 200px;
    position: absolute;
    left: 400px;
    bottom: 50px;
    z-index: 1;
}
.decoration2{
    position: absolute;
    width: 29%;
    left: -20%;
    bottom: 50%;
}
.circle{
    border: solid 4px #c3c3a7;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    position: absolute;
    top: 0;
    right: 0;
}
.img-container-background{
    background-image: url(../../assets/img/underlay-shape-grey.svg);
    background-repeat: no-repeat;
    background-size: 450px;
    background-position-y: bottom;
    background-position-x: left;
    width: 597px;
}

.star-now-button{
    padding: 10px;
    background-color: #20ad96;
    text-align: center;
    transition-duration: 0.3s;
    border-radius: 7px;
    width: 60%;
    &:hover{
        background-color: #3f3a64;
    }
}
.star-now-button a{
    text-decoration: none;
    color: #ffffff;
    font-weight: bolder;
}
</style>