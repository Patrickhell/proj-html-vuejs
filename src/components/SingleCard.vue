<template>
    <div class="card border-0  " style="height: 150px;" >
        <div class="row g-0">
            <div class="col-4 my-3 zoom-effect" >
                <img :src="getImagePath(cardElement.image)" alt="image" style="width: 150px;">
            </div>
            <div class="col-8 ">
                <div class="card-body  ">
                  <h5 class="card-title" style="color:#FEC96B ">{{ cardElement.subtitle }}</h5>
                  <p class="card-text" style="color:#667072">{{ cardElement.text }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'SingleCard',

    props:{
        cardElement:Object,
      
    },

    methods: {
        getImagePath: function(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        
      }
  
  }
    

}
</script>

<style lang="scss" scoped>
.card-title{
  font-size: 18px;
}
.card-text{
    font-size: 16px;
}
.zoom-effect:hover{
    -ms-transform: scale(1); 
    -webkit-transform: scale(1); 
    transform: scale(1.1);
    color: white;
    cursor: pointer;
}

</style>

