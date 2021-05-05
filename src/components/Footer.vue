<template>
     <section>
         <div class="container flex">

             <!-- dc comics & shop -->
             <div>
                <ul>
                    <h3> dc comics</h3>
                    <li v-for= "(item, index) in dsComics" :key= "index">
                        <a href="#"> {{ item.text }}</a></li>
                </ul>

                <ul>
                    <h3>shop</h3>
                    <li v-for= " (item,index) in shop " :key= "index"><a href="#"> {{item.text }}</a></li>
                </ul>
             </div>   

             <!-- dc -->
             <ul>
                 <h3>dc</h3>
                 <li v-for= "(item,index) in dc" :key= "index"><a href="#">{{ item.text }}</a></li>
             </ul>
             
             <!-- sites -->
             <ul>
                 <h3>sites</h3>
                 <li v-for= "(item,index) in sites" :key= "index" ><a href="#">{{ item.text }}</a></li>       
             </ul>
             
        </div>

         <!-- logo bg -->
         <div class="box">
            <img src="../assets/img/dc-logo-bg.png" alt="logo-bg">
         </div>
         
     </section>
  
</template>

<script>
export default {
    name: "Footer",
    data() {
        return {
            dsComics: [
                {text: "characters"},
                {text: "comics"},
                {text: "movies"},
                {text: "tv"},
                {text: "games"},
                {text: "videos"},
                {text: "news"},
            ],
            shop: [
                {text: "Shop DC"},
                {text: "Shop DC Collectibles"},
            ],
            dc: [
                {text: "terms Of Use"},
                {text: "Privacy policy (New)"},
                {text: "Ad Choise"},
                {text: "Jobs"},
                {text: "subscriptions"},
                {text: "Talent Workshops"},
                {text: "CPSC Certificates"},
                {text: "Ratings"},
                {text: "Shop Help"},
                {text: "Contact Us"},
            ],
            sites: [
                 {text: "DC"},
                 {text: "MAD Magazine"},
                 {text: "DC Kids"},
                 {text: "DC Universe"},
                 {text: "DC Power Visa"},
            ],

        }
    }
}
</script>

<style scoped lang="scss">
// importo variabili di stile
@import "../style/vars.scss";

section{
    position: relative;
    background-image: url(../assets/img/footer-bg.jpg); 
    
}

.container{
    padding: 60px 0;
}

/* LINKS */

ul{
    list-style: none;
     padding: 20px;   
} h3 {
    margin-bottom: 5px;
    color: $secondary;
    text-transform: $textTrasform;
} a{
    color: $footerLink;
    text-decoration: none;
    text-transform: capitalize;
    font-size: $font;
    transition: .3s;
    &:hover{
        color:$secondary;
    }
} 


/* LOGO BG */

.box{
    width: 530px;
    height: 425px;
    overflow: hidden;
    position: absolute;
    top: 0;
    left: 50%;
  
} img {
      width: 530px; 
}

</style>