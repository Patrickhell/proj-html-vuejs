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
                        <div class="btn-aboutMission">
                            <button class="btn-ourMission mb-4">
                              OUR MISSION
                            </button >
                        </div>
                        


                    </div>
                </div>
                <div class="rightSide col-4 " style="background-color:#ED6967 ;">
                    <div class="counter  text-white text-center">
                        <div class="d-flex justify-content-center ">
                            <h1>
                                <i class="fa-regular fa-heart " style="color:white"></i>
                            </h1>
                            <h2 class="numberFont">
                                2032
                            </h2> 
                        </div>
                        <p class="fontText">
                           Volunteers worldwide
                        </p>
                        <div class="d-flex justify-content-center">
                            <h1>
                                <i class="fa-solid fa-earth-americas"></i>
                            </h1>
                            <h2 class="numberFont">
                                 132
                            </h2>  
                        </div>
                        <p  class="fontText">
                            Active projets
                        </p>
                        <div class="d-flex justify-content-center">
                            <h1>
                                 <i class="fa-sharp fa-solid fa-dollar-sign"></i>
                            </h1> 
                            <h2 class="numberFont">
                                3.8M
                            </h2>  
                        </div>
                        <p  class="fontText">
                           Donated
                        </p>
                    </div>                  
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
                    <i class="fa-solid fa-droplet icons color-gold" ></i>
                </li>
                <li class=" value mb-4">
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
                <li class="buttonLearnMore">
                    <button class="btn-learnMore mb-4 m-auto">
                        LEARN MORE
                    </button >
                </li>
                
            </ul>
            <ul class="text-center">
                <li class=" mb-5 hover-icons">
                    <i class="fa-solid fa-stethoscope icons color-gold"></i>
                </li>
                <li class=" value mb-4">
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
                <li class="buttonLearnMore">
                    <button class="btn-learnMore mb-4 m-auto">
                          LEARN MORE
                    </button >
                </li>
                
            </ul>
            <ul class="text-center">
                <li class="mb-5 hover-icons">
                    <i  class="fa-solid fa-graduation-cap icons color-gold"></i>
                </li>
                <li class=" value  mb-4">
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
                <li class="buttonLearnMore">
                    <button class="btn-learnMore mb-4 m-auto">
                          LEARN MORE
                    </button >
                </li>
                
            </ul>
            <ul class="text-center mb-5">
                <li class="mb-5 hover-icons">
                    <i class="fa-brands fa-pagelines icons color-gold" ></i>
                </li>
                <li class=" value  mb-4">
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
                <li class="buttonLearnMore">
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
    <div class=" stripeForText  container-fluid text-white text-center d-flex bg-pink" style="height:150px;">
         <h4 class="m-auto viewCausesText">
            VIEW ALL OUR CAUSES
         </h4>
    </div>
    <div class="text-center">
        <div class="subtitle">
            <h1 class="mb-5">
              LATEST ARTICLES
            </h1>
            <div class="small-rule m-auto mb-5"></div>
            <h4 class="mb-5 " style="color:#737c7e">
                Together we make all the difference
            </h4>
        </div>
        <div class="containerForArticles text-start ">
            <div class="col-12 mb-5">
                <div class="row">
                    <div class="col-7 ">
                        <div class="card " style="width: 600px; border-radius: 0%;">
                            <div class="big-imageCard">
                                <img src="../assets/img/HelloIMG1669149322752.jpeg"  alt="...">
                                <div class="overlay">
                                    <p class="text">
                                       Understanding community complexities
                                    </p>
                                </div>
                            </div>                           
                            <div class="card-body ">
                              <h4 class="card-text" style="color:#FEC96B"> Understanding community complexities</h4>
                              <p style="color:#667072"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Prasent ac <br>
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
            <div class=" stripeForText text-white text-center d-flex mb-5 bg-pink" style="height: 50px;" >
                <h4 class="m-auto">
                  VIEW ALL OUR ARTICLES
                </h4>
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

 div.rightSide{
    background-image: url('../assets/img/home-content-bg-1.jpg');
   background-size: contain;
  background-position-y:center;
  position:relative;

 }
 .bg-pink{
    background-color: #ED6967 ;
    display: none;
 }
 div.counter{
    position:absolute;
    top: 50%;
    left:50%;
    transform:translate(-50%, -50%);
 }

 .fa-earth-americas, .fa-dollar-sign, .fa-heart{
    color:white; 
    font-size: 50px;
    margin-right: .5rem;
 }
 
 p.fontText{
    font-size: 22px;
    margin-bottom: 4rem;
 }
 h2.numberFont{
    font-size: 55px;
 }

 div.ourValueContent{
   background-image: url('../assets/img/HelloIMG1444664597507.jpg');
  background-position-x: center;
  background-position-y:65%;
 height: 950px;
 position: sticky;
 right:0;
 left:0;

 }
 div.ourValues{
    margin-bottom: 5rem;
 }

 ul li .icons{
    font-size: 50px;
    cursor: pointer;
 }

 .color-gold{
    color: #FEC96B;

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
 .containerForArticles{
  width:1150px;
  margin: 0 auto;
}
.big-imageCard{
    position:relative
 }
 


/** STARTED HOVER ELEMENTS */
div.btn-aboutMission:hover .btn-ourMission{
    background-color: #262E44;
 } 

 .stripeForText:hover{
    background-color: #408292;
    display: block;
 }
 .hover-icons:hover .color-gold{
    color:white
 }

 li.buttonLearnMore:hover .btn-learnMore{
    background-color: #262E44;
 }

 .overlay{
    position: absolute;
      right: 0;
      left: 0;
      bottom: 0;
  width: auto;
  height: 100%;
  transform: scaleX(0);
  transition: .3s ease-out;
 }

 .card:hover .overlay{
    transform: scaleX(1);
    background-color:rgba(254,201,107,0.6);
 }
 .big-imageCard:hover .overlay{
    transform: scaleX(1);
    background-color:rgba(254,201,107,0.6);
 }

 .text {
  color: white;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  width: 100%;
  
}


</style>