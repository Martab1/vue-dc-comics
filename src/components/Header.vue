<template>
    <header>

        <div class="container flex">
            <!-- logo -->
            <img src="../assets/img/dc-logo.png" alt="logo">

             <!-- links  -->
            <nav class="flex grow">
                <ul class="flex" >
                    <li v-for= "(link,index) in links" :key= "index"> 
                    <a :class= "{ active: link.current }" :href="link.url">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>

    </header>
  
</template>


<script>
// importo data
import headerLinks from "@/data/headerLinks.js";

export default {
    // nome componente
    name: "Header",
    data() {
       return {
           links: headerLinks,
       }
    }
}
</script>


<style scoped lang="scss">
// importo variabili di stile
@import "../style/vars.scss";

/* LOGO */
img{
    align-self: center;
    max-width: 70px;
}

/* NAV */
li { 
    padding: 45px 16px;
    list-style: none;
    a{
        text-decoration: none;
        text-transform: $textTrasform;
        font-size: $font;
        font-weight: bold;
        color: rgb(58, 57, 57);  
        transition: color .3s; 
        &.active,
        &:hover{
            color: $primary;
        }
    }
}



</style>