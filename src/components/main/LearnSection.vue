<template>
<div>
    <FirstContainerImg :benefits='benefits' />
    <SecondContainerImg />
</div>
</template>

<script>
import FirstContainerImg from "./FirstContainerImg"
import SecondContainerImg from './SecondContainerImg'
export default {
    components:{
        FirstContainerImg,
        SecondContainerImg
    },
    data:function () {
        return{
            benefits:[
                {
                    text:'Select & customize courses to your preferences'
                },
                {
                    text:'Change the tutor and make arrangements'
                },
                {
                    text:'Participate in events to join others'
                },
                {
                    text:'Get the disired certificaate delivdred at house'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">

</style>