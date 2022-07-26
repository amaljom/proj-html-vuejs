<template>
  <div class="d-flex">
    <div> <img class="w-50" src="../assets/dark-logo.png" alt=""> </div>
    <div>
        <!-- lista -->
        <div>
            <ul>
                <li v-for="(element, index) in navBarElements" :key="index"> {{ element.item}} </li>
            </ul>
        </div>
        <!-- icons -->
        <div>
            <span> <i class="fa-solid fa-cart-shopping"></i> </span>
            <span> <i class="fa-regular fa-user p-1"></i> </span>
        </div>
        <!-- seard -->
        <div>
            <div class="input-dec">
                <input type="text" name="" placeholder="Search...">
                <i class="fa-solid fa-magnifying-glass text-secondary"></i>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data: function(){
        return {
            navBarElements:[
                {
                    item:'Home'
                },
                {
                    item:'Pages'
                },
                {
                    item:'Courses'
                },
                {
                    item:'Features'
                },
                {
                    item:'Blog'
                },
                {
                    item:'Shop'
                },
                
            ]
        }
    },
}
</script>

<style lang="scss">
.input-dec{
    padding: 10px;
    background-color: white;
    border-radius: 6px;
}
input{
    border: 0;
    padding: 0;
    width: 8rem;
    outline: none;
}
</style>