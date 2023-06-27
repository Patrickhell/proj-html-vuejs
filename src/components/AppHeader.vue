<template>
    <header>
        <div class="container-fluid d-flex  text-white">
            <img class="logo" src="../assets/img/HelloIMG1669149314369.png " alt="logo_charity" style="width: 300px;"  >
            <ul class="  d-flex ">
                <li class="link" >
                  <a href="#" style="color:#FEC96B;">
                    HOME
                  </a>
                </li>
                <li class="link ">
                  <a href="#">
                    MISSION
                  </a>
                </li>
                <li class="dropdown link">
                    <p  class=" dropdown-toggle"  data-bs-toggle="dropdown" aria-expanded="false">
                        <a href=""> CAUSES</a>
                    </p>
                    <ul class="dropdown-content">
                        <li><a class="dropdown-item" href="#">FAIR TRADE</a></li>
                        <li><a class="dropdown-item" href="#">FARMING</a></li>
                        <li><a class="dropdown-item" href="#">VACCINES</a></li>
                        <li><a class="dropdown-item" href="#">EDUCATION</a></li>
                        <li><a class="dropdown-item" href="#">CLEAN WATER</a></li>
                        <li><a class="dropdown-item" href="#">SHELTER</a></li>
                    </ul>
                </li>
                <li class=" link" >
                   <a href="#">
                     JOURNAL
                   </a>
                </li>
                <li class="aboutDonate">
                   <button class="btn-donate">
                     DONATE
                   </button>
                </li>
        
            </ul>

        </div>
        <div class="text-white text-center ">
            <h1 class="mb-4">
               MAKE A DIFFERENCE
            </h1>
            <h5 class="mb-5">
               As long as poverty, injustice & inequality persit, none of us can truly rest.
            </h5>
            <div class="d-flex justify-content-center">
                <div class="button_aboutMission ">
                    <button class="btn-ourMission bg-transparent">
                     OUR MISSION
                    </button >
                </div>
                <div class="button_aboutDonate ">
                   <button class="btn-donateNow bg-transparent" >
                    DONATE NOW
                   </button>
                </div>
            </div>
            
            
           
        </div>
       
 
 

    </header>
   
</template>

<script>

export default {
    name: 'AppHeader',

        data(){
            return{

            }
        }
    }
    
</script>

<style lang="scss" scoped>

header{
    background-image: url('../assets/img/HelloIMG1669149393797.jpeg');
    height: 650px;
    background-size: cover;
    background-attachment:fixed;
}

.link{
    margin-right: 3.5rem;
    margin-top:6.5rem
}


.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f1f1f1;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}
li a{
    margin-top: 2rem;
    text-decoration: none;
    color: white;
}

.dropdown-content a:hover {
    background-color: #ddd;
}

.dropdown:hover .dropdown-content {
    display: block;
}

div img.logo{
   margin: 5.5rem;
  
}
li button{
    width: 130px;
    height: 45px;
    background-color: #FEC96B;
    border: none;
    margin-top: 6rem;
    color: white;
}
h1{
    width: 100%;
    font-size: 70px;
}

.btn-ourMission, .btn-donateNow{
    width: 190px;
    height: 45px;
    margin-right: 1.5rem;
    color: white;
    
}

.btn-donateNow{
    border:2px solid#FEC96B ;
   
}

.btn-ourMission{
border: 2px solid white;

}

.aboutDonate:hover .btn-donate{
    background-color:#262E44 ;

}
.button_aboutMission:hover .btn-ourMission{
    border:2px solid#FEC96B ;
    color: #FEC96B;
}

.button_aboutDonate:hover .btn-donateNow{
    color:white;
    border: 2px solid white;
    background-color: #262E44;

}
.link a:hover{
    color: #FEC96B;
}


</style>