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
    <div>
        <div class="card-lesson">
            <div class="w-100 position-relative">
                <img class="w-100 rounded-top" src="../assets/course-02-480x298.jpg" alt="">
                <div class="btn btn-primary position-absolute top-0 end-0">Free</div>
            </div>
            <div>
                <!-- name and photo -->
                <div class="d-flex">
                    <div class="img-container">
                        <img class="w-100" src="../assets/73ee246daf47502812ccefc84bf02898 (1).jpeg" alt="">
                    </div>
                    <p>name</p>
                </div>
                <!-- rest of the content -->
                <p>Learning to write as a professional author</p>
                <div class="d-flex">
                    <div>
                        <span><i class="fa-solid fa-file-lines"></i>&nbsp;</span>
                        <span>20 Lessons&nbsp;</span>
                    </div>
                    <div>
                        <span><i class="fa-solid fa-user"></i>&nbsp;</span>
                        <span>50 Students&nbsp;</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

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
    width: 30%;
    border-radius: 7px;
}
.img-container{
    width: 35px;
}
.img-container img{
    border-radius: 50%;
}
</style>