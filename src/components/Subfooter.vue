<template>
    <section>
        <!-- footer -->
        <div class="footer">

            <!-- button sign-up -->
            <div class=" container flex">
                <button>sign-up now!</button>

               <!-- social -->
                <div class="flex grow">
                    <ul class="flex">
                        <h4>follow us</h4>
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="fb"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a></li>
                        <li><a > <img src="../assets/img/footer-youtube.png" alt="youtube"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="locator"></a></li>
                    </ul>
                </div>

            </div>

        </div> 

    </section>
  
</template>

<script>
export default {
    name: "Subfooter",

}
</script>

<style scoped lang="scss">
@import "../style/vars.scss";

.footer{
    padding: 40px;
    background: rgb(46, 43, 43);     
}

/* BUTTON */
 button{
     cursor: pointer;
     background: transparent;
     padding: 12px;
     border: 2px solid $primary;
     text-transform: $textTrasform;
     color: #fff;
     position: relative;
     bottom: 5px;
     transition: .4s;
     &:hover{
         background:#fff;
         color: $primary;
     }
 }

 

/* SOCIAL */

h4{
    color: $primary;
    text-transform: uppercase;  
    position: relative;
    top: 8px;
    right: 20px;
}


li{
    margin: 0 10px;
    list-style: none;
}    

 
img{
    max-width: 30px;
}


</style>