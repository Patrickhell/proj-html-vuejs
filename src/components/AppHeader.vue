<template>
    <header>
        <div class="navBar container-fluid d-flex justify-content-between  text-white">
            <img class="logo" src="../assets/img/HelloIMG1669149314369.png " alt="logo_charity" style="width: 300px;"  >
            <ul class=" navBarRightSide d-flex ">
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
                    <div class="d-flex ">
                        <a href="#" class="m-auto">CAUSES</a>
                        <i class="fa-solid fa-angle-down mx-1 m-auto"></i>
                    </div>
                    <div class="dropdown-content">
                       <a class="items " href="#">FARMING</a>
                       <a  class="items " href="#">VACCINES</a>
                       <a  class="items " href="#">EDUCATION</a>
                       <a  class="items " href="#">CLEAN WATER</a>
                       <a  class="items " href="#">SHELTER</a>
                    </div>
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
        <div class="text-white text-center header-title me-auto">
            <h1 class="mb-4" >
                MAKE A DIFFERENCE
            </h1>
            <h6 class="mb-5 ">
                As long as poverty, injustice & inequality persit, none of us can truly rest.
            </h6>
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
     background-position-x: center;
     height:800px;
     background-position-y:80% ;
    background-size: cover;
    background-attachment:fixed;
}

.navBarRightSide{
    padding-right: 7rem;
}

.header-title{
    margin-top:7%;
    
  


}
div img.logo{
   margin: 3rem; 
}

h1{
    width: 100%;
    font-size: 70px;
}

li button{
    width: 130px;
    height: 45px;
    background-color: #FEC96B;
    border: none;
    margin-top: 4rem;
    color: white;
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

.link{
    margin-right: 3.5rem;
    margin-top:4.5rem
}

a{
   margin-top: 2rem;
   text-decoration: none;
   color: white;
}
.dropdown {
  position: relative;
  display: inline-block;
}
.dropdown-content a {
  color: black;
  padding: 10px ;
  text-decoration: none;
  display: block;
  text-align:left;
  width: 150px;
  line-height: 20px;
}
.dropdown-content a:hover{
    background-color:rgba(254,201,107,0.6);
}
.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f1f1f1;
  z-index: 1;
}


/** STARTED HOVER ELEMENTS */

.dropdown:hover .dropdown-content {
    display: block;
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