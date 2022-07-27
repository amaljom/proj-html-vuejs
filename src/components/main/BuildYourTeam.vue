<template>
  <div class="card-contenitore mt-5 pt-3 text-center">
    <div>
        <p class="color-special">START LEARNING CODING LANGUAGES</p>
    </div>
    <div class="d-flex justify-content-center">
        <h1 class="font-w-h1">Build your dream&nbsp;</h1>
        <h1>TODAY</h1>
    </div>
    <!-- inserisco i 4 component dinamicamente -->
    <div class="d-flex justify-content-around my-5">
        <div class="px-3" v-for="(element, index) in elements" :key="index">
            <img :src="require(`../../assets/img/${element.img}`)" alt="">
            <h5>{{ element.name }}</h5>
            <p> {{element.info}} </p>
            <div class="star-now-button">
                <a @click.prevent :href="`${element.url}`">Start now&nbsp;&nbsp;&nbsp;<i class="fa-solid fa-arrow-right-long"></i></a>
            </div>
            
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data:function(){
        return {
            elements:[
                {
                    img:'home-5-image-box-01.png',
                    name: 'Idea Discussione',
                    info: 'Get teamed up with the specialists ow work and teach coding for years at famous universities.',
                    url: '#'
                },
                {
                    img:'home-5-image-box-02.png',
                    name: 'Web Development',
                    info: 'Learn to start building a webpage from scratch. You decide your own pace, course and speed.',
                    url: '#'
                },
                {
                    img:'home-5-image-box-03.png',
                    name: 'System Administration',
                    info: 'Learners are encouraged to study tge mechanism and structure of system administration.',
                    url: '#'
                },
                {
                    img:'home-5-image-box-04.png',
                    name: 'Graphic Design',
                    info: 'Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss" scoped>
@import"../../assets/style/Variable.scss";
.color-special{
    color:#696b86;
}
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
}
.font-w-h1{
    color: $SectionsTitleColor;
    font-size: 3rem;
    font-weight: bolder;
}
h1{
    font-size: 3rem;
    color: $SectionsTitleColorSecondary;
}
h5{
    font-weight: bolder;
}
.star-now-button{
    padding: 10px;
    background-color: #ffffff;
    margin: 0 auto;
    widows: 80%;
    transition-duration: .3s;
    border-radius: 15px;
    &:hover{
        background-color: #f8f8f8;
    }
}
.star-now-button a{
    text-decoration: none;
    color: #8e8ba4;
    font-weight: bolder;
}
</style>