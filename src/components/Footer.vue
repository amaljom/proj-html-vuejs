<template>
<div>
    <div class="card-contenitore d-flex justify-content-around">
            <!-- left -->
            <div>
                <p class="fw-bold fs-4">Adress</p>
                <ul>
                    <li v-for="(element, index) in addresses" :key="index"> <a @click.prevent href="">{{element.text}}</a>  </li>
                </ul>
            <!--social icons -->
                <div>
                    <a @click.prevent href=""> <i class="fs-4 pe-5 fa-brands fa-square-facebook"> </i> </a> 
                    <a @click.prevent href=""> <i class="fs-4 pe-5 fa-brands fa-instagram"> </i></a>
                    <a @click.prevent href=""> <i class="fs-4 pe-5 fa-brands fa-twitter"> </i></a>
                    <a @click.prevent href=""> <i class="fs-4 pe-5 fa-brands fa-linkedin"> </i></a>
                </div>
            </div>
            <!-- right -->
            <div class="d-flex">
                <div class="px-4">
                    <p class="fw-bold fs-4">Explore</p>
                    <ul>
                        <li v-for="(element, index) in info" :key="index"><a @click.prevent href=""> {{element.inf}} </a></li>
                    </ul>
                </div>
                <div class="px-4">
                    <ul class="special-padding">
                        <li v-for="(element, index) in NotDefined" :key="index"> <a @click.prevent href=""> {{element.moreInfo}}</a></li>
                    </ul>
                </div>
                <div class="px-4">
                    <p class="fw-bold fs-4">Information</p>
                    <ul>
                        <li v-for="(element, index) in Explore" :key="index"><a @click.prevent href=""> {{element.Exp}} </a> </li>
                    </ul>
                </div>
            </div>
    </div>
    <div> <p class="fw-bold rights">2020 MaxCoach.All Rigts Reserved</p></div>
    <div>
       <a href="#ancora"> <i class="fa-solid fa-arrow-up anchor"></i></a> 
    </div>
</div>
</template>

<script>
export default {
    data:function(){
        return{
            addresses:[
                {
                    text:'382 NE 191st St # 87394 Mianmi, FL 33179-3899'
                },
                {
                    text:'+1(305)547-9909(9am-5pm ESTm Monday - Friday)'
                },
                {
                    text:'support@maxcoach.com'
                }
            ],

            info:[
                {
                    inf:'Start here'
                },
                {
                    inf:'Blog'
                },
                {
                    inf:'About us'
                },
            ],

            Explore:[
                {
                    Exp:'Memebership'
                },
                {
                    Exp:'Purchase guide'
                },
                {
                    Exp:'Privacy policy'
                },
                {
                    Exp:'Terms of service'
                },

            ],
            NotDefined:[
                {
                    moreInfo:'Success'
                },
                {
                    moreInfo:'Courses'
                },
                {
                    moreInfo:'Contact us'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import"../assets/style/Variable.scss";
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 80px;
    background-color: white;
}
ul{
    padding: 0;
}
ul li{
    list-style: none;
    padding: 8px 0px;
    font-weight: bold;
}
a, i {
    text-decoration: none;
    color: $FooterTextColor;
    &:hover{
        color: black;
    }
}
.rights{
    color: $FooterTextColor;
    text-align: center;
    padding: 40px 0px;
}
.special-padding{
    padding-top: 50px;
}
.anchor{
    font-size: 2rem;
    padding: 10px;
    position: relative;
    left: 95%;
    bottom: 57px;
    background: rgb(192, 192, 138);
    border-radius: 42%;
    width: 44px;
    height: 51px;
}
</style>