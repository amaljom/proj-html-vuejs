<template>
    <div class="background">
        <div class="card-contenitore pt-5">
            <div class="text-center py-5">
                <span class="color-special">GET IN CONTACT NOW</span>
                <!-- title -->
                <div class="d-flex justify-content-center">
                    <h1>Upcoming&nbsp;<span class="thinner">Events</span></h1>
                </div>
            </div>
            <div class="pt-5 mt-5 row justify-content-around ">
                <div v-for="(person, index) in people" :key="index" class="text-center card-member">
                    
                    <div class="profile-pic"> <img :src="require(`../../assets/img/${person.img}`)" alt=""> </div>
                    
                    <p class="info">
                        {{person.info}}
                    </p>
                    <p class="fw-bold">
                        {{ person.name }}
                    </p>
                    <span> {{ person.profession}} </span>
                </div>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
    data:function(){
        return{
            people:[
                {
                    img:'testimonial-avata-02.jpg',
                    info:'I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.',
                    name:'MINO HOLLACE',
                    profession:'/Freelancer'
                },
                {
                    img:'testimonial-avata-01.jpg',
                    info:'MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.',
                    name:'MADLEY PONDOR',
                    profession:'/IT Specialst'
                },
                {
                    img:'testimonial-avata-04.jpg',
                    info:'I am happy with their arrangerment of lessons and subject. They reflect a scientific investigation.',
                    name:'LUVIC DUBBLE',
                    profession:'/Private Tutor'
                }
            ]
        }
    }
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
.background{
    background-color: #f3f3f3;
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
.card-member{
    width:30%;
    background-color: white;
    position: relative;
    padding: 65px 30px;
    border-radius: 6px;
}
.profile-pic{
    width: 130px;
    position: absolute;
    bottom: 80%;
    left: 32%;
}

.profile-pic img{
    width:100% ;
    border-radius: 50%;
}
.info{
    color: $SectionsTitleColor;
}
.card-member span{
    color: $SectionsTitleColorSecondary ;
}
</style>