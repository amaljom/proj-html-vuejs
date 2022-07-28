<template>
    <div class="card-contenitore d-flex justify-content-between my-5 py-3 background-container" >
        <div class="img-container-background"> <img src="../../assets/img/about-us-03-image-01.png" alt=""> </div>
        
        <div class="container-size">
            <!-- prima del titolo -->
            <span class="color">DREAM WITH&nbsp;</span>
            <span class="fw-bold color">MAXCOACH</span>
            <!-- titolo -->
            <div class="d-flex">
                <h1>Construct A&nbsp;</h1>
                <h1 class="thinner">Stunning</h1>
            </div>
                <h1>Carreer Prespective</h1>
            <!-- tre div contenente i tre oggetti -->
            <div class="outer-box mt-5">
                <div class="inner-box">
                    <span>Multiple Platforms Supported for Teaching & Studying</span>
                    <i class="fa-solid fa-circle-minus"></i>
                </div>
                <p>MaxCoach supports the asct of teaching and learning on multiple platforms like online or offline via marterial downloads.
                    We know things aren't supposed to be devoureed in a short time, you can always access our knowledge base from any device.
                </p>
            </div>

            <div class="outer-box-special my-4">
                <span>Multiple Platforms Partecipation at the Same Time</span>
                <i class="fa-solid fa-circle-plus"></i>
            </div>
            
            <div class="outer-box-special">
                <span>Track Study Progress & Deliver Prompt Feedback</span>
                <i class="fa-solid fa-circle-plus"></i>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
@import"../../assets/style/Variable.scss";
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
}
.color{
    color:$ElementOverTitles;
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
    width: 50%;
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
    width: 370px;
    position: relative;
    left: 164px;
}
.img-container-background{
    background-image: url(../../assets/img/underlay-shape-lilla.svg);
    background-repeat: no-repeat;
    background-size: 410px;
    background-position-y: bottom;
    width: 487px;
}
.outer-box{
    background-color: rgb(255, 255, 255);
    border-radius: 7px;
    width: 91%;
    -webkit-box-shadow: 0px 12px 42px -7px #000000;
    -moz-box-shadow: 0px 12px 42px -7px #000000;
    -o-box-shadow: 0px 12px 42px -7px #000000;
    box-shadow: 0px 6px 24px -8px #ffaaaa;
}

.inner-box{
    display: flex;
    padding: 12px;
    background-color: #62c5b5;
    align-items: center;
    justify-content: space-between;
    border-top-right-radius: 7px;
    border-top-left-radius: 7px;
}
.inner-box span, .inner-box i{
    font-weight: bolder;
    color: #fff;
}
.outer-box p{
    padding: 30px;
}
.outer-box-special{
    background-color: rgb(255, 255, 255);
    border-radius: 7px;
    width: 91%;
    -webkit-box-shadow: 0px 12px 42px -7px #000000;
    -moz-box-shadow: 0px 12px 42px -7px #000000;
    -o-box-shadow: 0px 12px 42px -7px #000000;
    box-shadow: 0px 6px 24px -8px #ffaaaa;
    padding: 10px;
    display: flex;
    justify-content: space-between;
}
</style>