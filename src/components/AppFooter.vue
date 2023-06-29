<template>
    <div class="container-fluid text-center text-white mb-5">
        <div class="bg-image">
            <div class="subtitle">
                <h1 class="mb-5">
                    CHANGE A LIFE TODAY
                </h1>
                <div class="small-rule m-auto mb-5"></div>
                <h5 class="mb-5 " >
                    As long as poverty, injustice & inequality persist, none of us can truly rest. It doesn’t <br>
                     take much to change a life, Get in touch today and start making the difference.
                </h5>
                <div class="d-flex justify-content-center">
                    <div class="button_aboutVolunteer  ">
                        <button class="btn-ourVolunteer bg-transparent">
                             VOLUNTEER
                        </button >
                    </div>
                    <div class="button_aboutDonateNow ">
                        <button class="btn-donateNow bg-transparent" >
                            DONATE NOW
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="d-flex p-4" >
        <img src="../assets/img/HelloIMG1669149314987.png" alt="" style="width: 250px;" class="m-auto">
    </div>
    <p class="text-center p-5">
        © Copyright 2012 - 2023 | Avada Theme by <a href="#" style="color:#FEC96B;">ThemeFusion</a> | All Rights Reserved | Powered by <a href="#" style="color:#FEC96B;">WordPress</a>
    </p>
    <ul class=" icons-socials d-flex justify-content-center fs-4 " >
        <li  class="social ">
            <i class="fa-brands fa-facebook-f  mx-3 "  style="color:#FEC96B"></i>
            <span class="tooltiptext">Facebook</span>
           
        </li>
        <li class="social " >
            <i class="fa-brands fa-instagram  mx-3 "  style="color:#FEC96B"></i>       
            <span class="tooltiptext">Instagram</span>
        </li>
        <li class="social" >
            <i class="fa-brands fa-twitter mx-3 "  style="color:#FEC96B"></i>           
            <span class="tooltiptext">Twitter</span>
        </li>
        <li class="social" >
            <i class="fa-brands fa-youtube mx-3 "  style="color:#FEC96B"></i>
            <span class="tooltiptext">Youtube</span>       
        </li>
    </ul>
    
    
    
  
</template>

<script>

export default {
    name: 'AppFooter',

        data(){
            return{

            }
        }
    }
    
</script>

<style lang="scss" scoped>
.bg-image{
    background-image: url('../assets/img/Avada-footer.jpg');
    background-position-x: center;
  background-position-y:center;
  background-size: cover;
  height: 550px;

}

.btn-ourVolunteer, .btn-donateNow{
    width: 190px;
    height: 45px;
    margin-right: 1.5rem;
    color: white;  
}
.btn-donateNow, .btn-ourVolunteer{
    border:2px solid white;  
}

a{
    text-decoration: none;
 }


/** STARTED HOVER ELEMENTS */

 .button_aboutVolunteer:hover .btn-ourVolunteer{
    border:2px solid #FEC96B;
}

.button_aboutDonateNow:hover .btn-donateNow{
    border:2px solid #FEC96B;
}

.social {
  position: relative;
  display: inline-block;
  cursor:pointer
}

.social:hover .tooltiptext {
  visibility: visible;
}

.social .tooltiptext {
  visibility: hidden;
  width: 80px;
  background-color: black;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  position: absolute;
  z-index: 1;
  bottom: 110%;
  left: -25%;
  font-size: 10px;
}
.social .tooltiptext::after {
    content: " ";
  position: absolute;
  top: 100%;
  left: 50%;
  margin-left: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: black transparent transparent transparent;
}

</style>