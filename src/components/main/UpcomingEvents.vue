<template>
<div>
    <div class="card-contenitore pt-5">
        <div class="text-center">
            <span class="color-special">GET IN CONTACT NOW</span>
            <!-- title -->
            <div class="d-flex justify-content-center">
                <h1>Upcoming&nbsp;<span class="thinner">Events</span></h1>
            </div>
        </div>
        <!-- card container -->
        <div class="row py-5">
            <div v-for="(card,index) in cards" :key="index" class="card-item">
                <!-- left -->
                <div>
                    <div class="pb-2">
                        <i class="fa-solid fa-location-dot pe-2"></i>
                        <span>{{card.place}}</span>
                    </div>
                    <div>
                        <span class="special-font-weigth">{{card.info}}</span>
                    </div>
                </div>
                <!-- right -->
                <div class="text-center">
                    <h1 class="thinner">{{card.date}}</h1>
                    <span class="m-0 special-font-weigth">{{card.month}}</span>
                    <ButtonComponent 
                    :url="card.url"
                    :buttonText="buttonTxt" />
                </div>
            </div>
        </div>
        <div class="text-center color-special">
            <span>Exited about our events?&nbsp;</span>
            <span><a @click.prevent href="#">View all events</a></span>
        </div>
    </div>
    <img class="wave" src="../../assets/img/wave2.svg" alt="">
</div>
</template>

<script>
import ButtonComponent from './ButtonComponent'
export default {
    components:{
        ButtonComponent
    },
    data:function(){
        return{
            cards:[
                {
                    place:'Texas, US',
                    info:'Storytelling Workshop',
                    date:22,
                    month:'NOV',
                    url:'#'
                },
                {
                    place:'New York, US',
                    info:'painting Art Contest 2020',
                    date:10,
                    month:'OCT',
                    url:'#'
                },
                {
                    place:'Hamburg, Germany',
                    info:'Intternational Art Fair 2020',
                    date:23,
                    month:'NOV',
                    url:'#'
                },
                {
                    place:'Illinois, US',
                    info:'Street Performance: Call for Artist',
                    date:15,
                    month:'DEC',
                    url:'#'
                },
                {
                    place:'Illinois, US',
                    info:'Consumero Food Safety Education Conference',
                    date:22,
                    month:'JUL',
                    url:'#'
                },
                {
                    place:'Dubai',
                    info:'How mediation improve your mental healt?',
                    date:12,
                    month:'AUG',
                    url:'#'
                }

            ],
            buttonTxt:"Get Ticket"
        }
    }
}
</script>

<style lang="scss" scoped>
@import"../../assets/style/Variable.scss";
.color-special{
    color:$ElementOverTitles;
}
.card-contenitore{
    width: $windowSize;
    margin: 0 auto;
    padding-top: 10px;
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
.card-item{
    display: flex;
    background-color: #fafafa;
    border-radius: 4px;
    padding: 20px 40px;
    justify-content: space-between;
    margin: 15px;
    width: calc((100% / 2) - 30px);
    transition-duration: .3s;
    &:hover{
        border-left: 2px solid #20ad96;
        background-color: white;
        box-shadow: 0px 6px 24px -8px #ffaaaa;
    }
}
.special-font-weigth{
    font-weight: bolder;
}
.color-special a{
    font-weight: bold;
    color: #20ad96;
}

.wave{
    transform: scaleY(-1);
    width: 100%;
    height: 310px;
    filter: invert(44%) sepia(194%) saturate(1351%) hue-rotate(316deg) brightness(334%) contrast(91%);
}
</style>