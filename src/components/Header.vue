<template>
  <header>
        <div class="card-contenitore div-position">
            <div class=" d-flex justify-content-between align-items-center">
                <div> <img class="w-50" src="../assets/dark-logo.png" alt=""> </div>
                
                <div class="d-flex align-items-center">
                    <!-- lista -->
                    <div>
                        <ul class="m-0">
                            <li v-for="(element, index) in navBarElements" :key="index"> {{ element.item}} <i class="fa-solid fa-angle-down font-icon"></i> </li>
                        </ul>
                    </div>
                    <!-- icons -->
                    <div >
                        <span class="px-2"> <i class="fa-solid fa-cart-shopping"></i> </span>
                        <span class="px-2"> <i class="fa-regular fa-user p-1"></i> </span>
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
            <!-- Creazione del component contente la grossa immagine -->
            <ContainerWithImg />
        </div>
        <div class="img-container"><img class="img-backgorund" src="../assets/jumbo-overlay.svg" alt="Non Trovato"></div>
  </header>
</template>

<script>
import ContainerWithImg from './ContainerWithImg'
export default {
    components: {
        ContainerWithImg
    },

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

<style lang="scss" scoped>
@import"../assets/style/Variable.scss";
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
}
header{
    background-color: #e9e6e3;
}

.input-dec{
    padding: 12px 10px;
    background-color: white;
    border-radius: 6px;
}
input{
    border: 0;
    padding: 0;
    width: 8rem;
    outline: none;
}
ul li{
    list-style: none;
    cursor: pointer;
    display: inline;
    padding: 25px ;
    color: #3f3a64;
}

.div-position{
    position: relative;
    z-index: 99;
}
.font-icon{
    font-size:10px;
}
.img-container{
    width: 100%;
    position: relative;
}
.img-backgorund{
    width: 100%;
    height: 400px;
    -webkit-transform: scaleY(-1);
    transform: scaleY(-1);
    position: absolute;
    bottom: 0;
}
</style>