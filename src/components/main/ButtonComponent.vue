<template>
     <div class="star-now-button">
        <a @click.prevent :href="`${url}`">{{ buttonText }}</a>
    </div>
</template>

<script>
export default {
    props:{
        url:String,
        buttonText:String
    }
}
</script>

<style lang="scss" scoped>
.star-now-button{
    padding: 10px;
    background-color: #20ad96;
    text-align: center;
    transition-duration: 0.3s;
    border-radius: 7px;
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