<template>
    <header>

        <div class="container flex">
            
            <img src="../assets/img/dc-logo.png" alt="">

            <nav class="flex">
                <ul class="flex" >
                    <li v-for= "(link,index) in links" :key="index"> 
                    <a href="#">{{ link.text }}</a></li>
                </ul>
            </nav>
       
        </div>
    </header>
  
</template>


<script>
export default {
    // nome componente
    name: "Header",
    data() {
       return {
           links: [
               { text: "characters", url: "/characters", current: false},
               { text: "comics", url: "/comics", current: true},
               { text: "movies", url: "/movies", current: false},
               { text: "tv", url: "/tv", current: false},
               { text: "games", url: "/games", current: false},
               { text: "collectilbles", url: "/collectibles", current: false},
               { text: "videos", url: "/videos", current: false},
               { text: "fans", url: "/fans", current: false},
               { text: "news", url: "/news", current: false},
               { text: "shop", url: "/shop", current: false},
           ],
       }
    }
}
</script>


<style scoped>

/* LOGO */
img{
    align-self: center;
    max-width: 70px;
}

/* NAV */
nav{
    flex-grow: 1;
    justify-content: flex-end;
}

li{
   padding: 45px 16px;
   list-style: none;
}

li a{
    text-decoration: none;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: bold;
    color: rgb(58, 57, 57);  
    transition: color .3s; 
}

li a:hover{
    color: rgb(66, 104, 206);
}





</style>