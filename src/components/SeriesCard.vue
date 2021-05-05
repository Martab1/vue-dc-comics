
<!-- creazione singola card -->
<template>
    <div class="box">
        <div class="img-box">
          <img :src="obj.thumb" :alt="obj.series">
        </div> 
        <h4> {{ obj.series }}</h4>
    </div>
</template>

<script>

export default {
    // nome componente
     name: "SeriesCard",
     // props = riferimento a ciò che mi passa l'array del componente padre
     props: ["obj"],
}
</script>

<style scoped>


.box{
    width: calc(90% / 6 );
    margin: 0 auto;
}

.img-box{
    height: 150px;
    overflow-y: hidden;    
}

img{
    height: 210px;
}

h4{
    padding: 20px 0;
    font-size: 13px;
    text-transform: uppercase;
    font-weight: 400;
}

</style>