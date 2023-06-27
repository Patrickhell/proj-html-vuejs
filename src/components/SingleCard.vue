<template>
    <div class="card border-0  " style="height: 150px;" >
        <div class="row g-0">
            <div class="col-4 my-3" >
                <img :src="getImagePath(cardElement.image)" alt="image" style="width: 150px;">
            </div>
            <div class="col-8 ">
                <div class="card-body  ">
                  <h5 class="card-title">{{ cardElement.subtitle }}</h5>
                  <p class="card-text">{{ cardElement.text }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'SingleCard',

    props:{
        cardElement:Object
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

</style>

