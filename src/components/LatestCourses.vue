<template>
  <div class="card-contenitore mt-5 pt-4 ">
    <div class="text-center">
        <p class="color-special">CHOOSE WHERE YOU'D LIKE TO BEGIN</p>
    </div>
    <div class="d-flex justify-content-center">
        <h1 class="font-w-h1">Latest Featured&nbsp;</h1>
        <h1>Courses</h1>
    </div>
    <!-- A DIV TO CONTAIN ALL CARDS -->
    <div class="row py-5">
        <div v-for="(card,index) in cards" :key="index" class="card-lesson">
            <div class="w-100 position-relative">
                <img class="w-100 rounded-top" :src="require(`../assets/${card.img}`)" alt="">
                <div class="costo position-absolute top-0 end-0"> {{card.price}} </div>
            </div>
            <div class="detail-container">
                <!-- name and photo -->
                <div class="d-flex align-items-center">
                    <div class="img-container">
                        <img class="w-100" :src="require(`../assets/${card.author}`)" alt="">
                    </div>
                    <span class="px-3">{{card.authorName}}</span>
                </div>
                <!-- rest of the content -->

                <p class="author">{{card.info}}</p>

                <div class="d-flex">
                    <div>
                        <span><i class="fa-solid fa-file-lines"></i>&nbsp;</span>
                        <span>{{card.lessons}} Lessons&nbsp;</span>
                    </div>
                    <div class="ps-4">
                        <span><i class="fa-solid fa-user"></i>&nbsp;</span>
                        <span>{{card.completedStudents}} Students&nbsp;</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data: function(){
        return{
            cards:[
                {
                    img:'course-02-480x298.jpg',
                    price:'$40.00',
                    author:'73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    authorName:'Balanche Fields',
                    info:'Learning to write as a professional author',
                    lessons:20,
                    completedStudents:50
                },
                {
                    img:'stock-full-hd-03-480x298.jpg',
                    price:'Free',
                    author:'d0d504142acfde820eef2f11feea6253 (1).jpeg',
                    authorName:'Maggie Strickland',
                    info:'Customer-centric info-Tech Strategies',
                    lessons:24,
                    completedStudents:749
                },
                {
                    img:'stock-full-hd-04-480x298.jpg',
                    price:'$19.00',
                    author:'d0d504142acfde820eef2f11feea6253 (1).jpeg',
                    authorName:'Maggie Stricklan',
                    info:'Open Programming Courses for Everyone: Python',
                    lessons:17,
                    completedStudents:62
                },
                {
                    img:'stock-full-hd-06-480x298.jpg',
                    price:'$26.00',
                    author:'73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    authorName:'Balanche Fields',
                    info:'Academic Listening and Note-taking',
                    lessons:14,
                    completedStudents:67
                },
                {
                    img:'course-featured-image-01-480x298.jpg',
                    price:'$39.00',
                    author:'73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    authorName:'Balanche Fields',
                    info:'Master jQuery in a Short Perio of Time',
                    lessons:6,
                    completedStudents:51
                },
                {
                    img:'stock-full-hd-05-480x298.jpg',
                    price:'$59.00',
                    author:'73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    authorName:'Balanche Fields',
                    info:'Introduction to Javascript for Beginners',
                    lessons:14,
                    completedStudents:76
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import"../assets/style/Variable.scss";
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
}
.color-special{
    color:#696b86;
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

// card
.card-lesson{
    width: calc( 100% / 3);
    border-radius: 7px;
}
.img-container{
    width: 35px;
}
.img-container img{
    border-radius: 50%;
}
.author{
    font-size: 1.3rem;
    font-weight: bold;
}
.detail-container{
    padding: 20px 45px;
}
.costo{
    width: 80px;
    background-color: rgb(84, 122, 84);
    text-align: center;
    padding: 10px;
    color: white;
    font-weight: bold;
    border-radius: 0px 7px;
}
</style>