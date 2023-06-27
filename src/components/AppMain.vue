<template>
    <div class="container-fluid">
        <div class="col-12">
            <div class="row">
                <div class="leftSide col-8 text-" >
                    <h1 class="mb-4">
                        EVERY MOMENT COUNTS
                    </h1>
                    <div class="small-rule"></div>
                    <div>
                        <p>
                         Curabitur non mi et turpis pharetra vulputate. Cras consequat, risus nec commodo vehicula,<br>
                         nisi est laoreet leo, ac convallis nisi nibh id velit. Aliquam mattis metus a nisi pretium.<br>
                        </p>
                        <p>
                           Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ac nibh vestibulum,<br>
                          laoreet ipsum quis, vestibulum nisi. Curabitur non mi et turpis pharetra vulputate. Ipsum <br>
                          dolor sit amet, consectetur adipiscing elit. Praesent ac nibh vestibulum, laoreet ipsum quis,<br>
                          vestibulum nisi.
                        </p>
                        <p class="mb-5">
                           Curabitur non mi et turpis pharetra vulputate. Cras consequat, risus nec commodo vehicula,<br>
                           nisi est laoreet leo, ac convallis nisi nibh id velit.
                        </p>
                        <button class="btn-ourMission mb-4">
                          OUR MISSION
                        </button >


                    </div>
                </div>
                <div class="rightSide col-4" style="background-color:#ED6967 ;">
                    <ul class="d-flex">
                        <li>
                            <i class="fa-regular fa-heart"></i>
                        </li>
                        <li>
                            2032
                        </li>
                    </ul>
                    <h3>
                        Volunteers worldwide
                    </h3>
                    <ul class="d-flex">
                        <li>
                            <i class="fa-solid fa-earth-americas"></i>
                        </li>
                        <li>
                            132
                        </li>
                    </ul>
                    <h3>
                        Active projets
                    </h3>
                    <ul class="d-flex">
                        <li>
                            <i class="fa-sharp fa-solid fa-dollar-sign"></i>
                        </li>
                        <li>
                            3.8M
                        </li>
                    </ul>
                    <h3>
                        Donated
                    </h3>
                </div>

            </div>

        </div>
    </div>
    <div class="container-fluid ourValueContent  text-center text-white">
        <div class="subtitle">
            <h1 class="mb-5">
              OUR VALUES
            </h1>
            <div class="small-rule m-auto mb-5"></div>
            <h4 class="mb-5">
                Think Big. Act Bigger.
            </h4>
        </div>
        <div class=" ourValues text-center d-flex justify-content-center">
            <ul >
                <li class="mb-5 hover-icons">
                    <i class="fa-solid fa-droplet icons" ></i>
                </li>
                <li class=" value text mb-4">
                    <h4 >
                      Clean water
                    </h4>
                </li>
                <li class="mb-5">
                    Nullam convallis, orci in <br>
                    congue aliquet, diam maurisbr <br>
                    cursus urna, Id maximus lectus <br>
                    magna maximus.
                </li>
                <li class="button">
                    <button class="btn-learnMore mb-4 m-auto">
                        LEARN MORE
                    </button >
                </li>
                
            </ul>
            <ul class="text-center">
                <li class=" mb-5 hover-icons">
                    <i class="fa-solid fa-stethoscope icons"></i>
                </li>
                <li class=" value text mb-4">
                    <h4>
                       Vaccinations
                    </h4>
                </li>
                <li class="mb-5">
                    Nullam convallis, orci in <br>
                    congue aliquet, diam maurisbr <br>
                    cursus urna, Id maximus lectus <br>
                    magna maximus.
                </li>
                <li class="button">
                    <button class="btn-learnMore mb-4 m-auto">
                          LEARN MORE
                    </button >
                </li>
                
            </ul>
            <ul class="text-center">
                <li class="mb-5 hover-icons">
                    <i  class="fa-solid fa-graduation-cap icons"></i>
                </li>
                <li class=" value text mb-4">
                    <h4 >
                        Education
                    </h4>
                </li>
                <li class="mb-5">
                    Nullam convallis, orci in <br>
                    congue aliquet, diam maurisbr <br>
                    cursus urna, Id maximus lectus <br>
                    magna maximus.
                </li>
                <li class="button">
                    <button class="btn-learnMore mb-4 m-auto">
                          LEARN MORE
                    </button >
                </li>
                
            </ul>
            <ul class="text-center mb-5">
                <li class="mb-5 hover-icons">
                    <i class="fa-brands fa-pagelines icons" ></i>
                </li>
                <li class=" value text mb-4">
                    <h4 >
                        Farming
                    </h4>
                </li>
                <li class="mb-5">
                    Nullam convallis, orci in <br>
                    congue aliquet, diam maurisbr <br>
                    cursus urna, Id maximus lectus <br>
                    magna maximus.
                </li>
                <li class="button">
                    <button class="btn-learnMore mb-5 m-auto">
                        LEARN MORE
                    </button >
                </li>
                
            </ul>
            
        </div>
    </div>
    <div class="container">
        <div class="text-center subtitle ">
            <h1 class="mb-4">
                RECENT CAUSES
            </h1>
            <div class="small-rule m-auto mb-5"></div>
            <h4 class=" mb-5" >
                We run projects in over 30 countries in 5 contintents
            </h4>
           
            <div class=" cards-content ">
                <article class="card " v-for="card in cardsList" :key="card">
                    <img :src="getImagePath(card.image)" alt="image" >
                    <div class="overlay">
                        <p class="text">
                            {{ card.text }}
                        </p>
                    </div>
                </article>

            </div>
        </div>
    </div>
    <div class="container-fluid text-white text-center d-flex " style="height: 150px; background-color:#ED6967">
         <h4 class="m-auto">
            VIEW ALL OUR CAUSES
         </h4>
    </div>
    <div class="text-center">
        <div class="subtitle">
            <h1 class="mb-5">
              LATEST ARTICLES
            </h1>
            <div class="small-rule m-auto mb-5"></div>
            <h4 class="mb-5 " style="color:gray">
                Together we make all the difference
            </h4>
        </div>
        <div class="container1 text-start ">
            <div class="col-12">
                <div class="row">
                    <div class="col-7 ">
                        <div class="card " style="width: 600px; border-radius: 0%;">
                           <img src="../assets/img/HelloIMG1669149322752.jpeg" class="card-img-top" alt="...">
                           <div class="card-body ">
                              <h4 class="card-text"> Understanding community complexities</h4>
                              <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac <br>
                                nibh vestibulum, laoreet ipsum.
                              </p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="flex-column col-5">
                       <CardsList />
                    </div>
                </div>
            </div>
        </div>
    </div>
   
</template>

<script>
import CardsList from './CardsList.vue';


export default {
    name: 'AppMain',
    components:{
        CardsList,
    },

        data(){
            return{
                cardsList :[
                {image:'HelloIMG1669149317319.jpeg',
                  text: 'FAIR TRADE'
                },

                {image:'HelloIMG1669149318263.jpeg',
                  text: 'SHELTER'
                }, 

                {image: 'HelloIMG1669149319450.jpeg',
                 text : 'FARMING'
                },

                {image :'HelloIMG1669149321401.jpeg',
                 text : 'VACCINES'
                }
                
               ]
                

            }
        },
       

        methods: {
        getImagePath: function(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        
      }
  
  }
    }

</script>

<style lang="scss" scoped>

div.leftSide{
    padding: 6rem ;
}
 div.small-rule{
    width: 190px;
    border :2px solid #FEC96B;
    margin-bottom: 3rem;
    
 }

 .btn-ourMission, .btn-learnMore{
    width: 160px;
    height: 45px;
    margin-right: 1.5rem;
    color: white;
    background-color:#FEC96B ;
    border:none
 }

 .fa-earth-americas{
    background-color: white;
    color:#ED6967 ;
 }

 div.ourValueContent{
   background-image: url('../assets/img/HelloIMG1444664597507.jpg');
  background-position-x: center;
  background-position-y:65%;
 height: 950px;

 }
 

 div.subtitle{
    padding-top:8rem;
 }

 ul li .icons{
    font-size: 50px;
    color: #FEC96B;
    cursor: pointer;
 }
 div.ourValues{
    margin-bottom: 5rem;
 }
 li.hover-icons:hover .icons{
    color: white;
 }
 li.value{
    cursor: pointer;
 }
 li.value:hover .icons{
    color: white;
    
 }
 li.button:hover .btn-learnMore{
    background-color: #262E44;

 }

 li.button:hover + .icons{
    color: white;
 }
 .container{
    width: 1000px;
    
 }
 .cards-content{
   width: 100%;
   display: flex;
   flex-direction: row;
   flex-wrap: wrap;
   margin-bottom: 6rem;

 }
 .card{
    width: calc((100% / 3) - 1.5rem);
    margin:.7rem ;
    position: relative;
   
 }
 img{
    width: 100%;
    object-fit: cover;
 }
 .overlay{
    position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
  background-position: center;
  width: 100%;
  height: 100%;
  transform: scale(0);
  transition:all .2s ease-out;
 }
 .card:hover .overlay{
    transform: scale(1);
    filter: brightness(1);
 }

 .text {
  color: white;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.container1{
    width:1150px;
    margin: 0 auto;
   
}


</style>