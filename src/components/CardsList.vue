<template>
    <SingleCard v-for="cardObj in cardsList" :key="cardObj"
                        :cardElement = "cardObj" />
  
</template>

<script>
import SingleCard from './SingleCard.vue';

export default {
    name:'CardsList',
    
        data(){
            return{ 
                  
                cardsList :[

                {
                    image:'HelloIMG1444664597500.jpg',
                    subtitle:'The human story of uniqueness',
                    text :'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.'
                },

                {
                    image:'HelloIMG1444664597501.jpg',
                    subtitle:'Sustainable trade tactics',
                    text :'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.'
                },

                {
                    image:'HelloIMG144466459750022.jpg',
                    subtitle:'Farmers making a difference',
                    text :'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.'
                },

                {
                    image:'HelloIMG14446645975002223.jpg',
                    subtitle:'Meeting remote tribes in Peru',
                    text :'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac nibh vestibulum, laoreet ipsum.'
                },

                ]
                

            }
            
        },
        components:{
            SingleCard,
        },

    }

</script>

<style>

</style>