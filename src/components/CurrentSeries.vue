<template>
   <section>
       <!-- title -->
       <div class="container"> 
           <h2>current series</h2>
       </div>

       <!-- series -->
       <div class="container flex images">
            <SeriesCard v-for= "(serie,index) in cards" :key= "index" :obj= "serie" /> 
       </div>

       <!-- load btn --> 
       <div class="container flex">
            <button>load more</button>
       </div>
       
   </section>
</template>

<script>

//import componente
import SeriesCard from "@/components/SeriesCard.vue"
//import data
import seriesCards from "@/data/seriesCards.js"

export default {
    //nome componente
     name: "CurrentSeries",
     //componenti che ne fanno parte
     components: {
         SeriesCard,
     },
     data(){
         return {
             cards: seriesCards,
                     
         }
     }
}
</script>

<style scoped lang="scss">
// importo variabili di stile
@import "../style/vars.scss";

section{
    background: $mainBg;
    color: $secondary;
}

.container{
    justify-content: center;
}

h2{
    display: inline-block;
    padding: 10px 30px;
    position: relative;
    bottom: 15px;
    text-transform: $textTrasform;
    font-size: 1.4rem;
    background: $primary;    
}

.images{
    flex-wrap: wrap;
    padding: 0 10px;
    padding-bottom: 40px; 
} 



button{
    cursor: pointer;
    padding: 10px 60px;
    text-transform: $textTrasform;
    color: $secondary;
    font-weight: bold;
    background: $primary;
    border: none;  
    margin-bottom: 30px;   
    transition: .4s;
    &:hover{
        color: $primary;
        background: $secondary;
    }
}



</style>