<template>
        <div class="row">
        <!--sidebox-->
        <div class="sidebox wrapper col-sm-12 col-md-12 col-lg-6 col-xl-6 col-xxl-6">

            <div class="animation p-0">
                <img class="crmslogo" src="../../src/assets/img/crms-transparent-logo.png" alt="CRMS">
            </div>

            <!--bubbles-->
            <section class="sticky">
                <div class="bubbles">
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                    <div class="bubble"></div>
                </div>
            </section>

        </div>
        <!--sidebar-->
        <div class="sidebar col-sm-12 col-md-12 col-lg-6 col-xl-6 col-xxl-6">

            <div class="row">
                <div class="col-sm-12 col-md-1 col-lg-2 col-xl-2 col-xxl-2"></div>
                <div class="col-sm-12 col-md-10 col-lg-8 col-xl-8 col-xxl-8">

                    <form id="login" class="mt-2 container loginbox float-start">
                        <div class="row-vertical">
                            <div class="col">
                                <div class="title mb-4 fw-bold">CRMS</div>
                                <h3 class="subtitle mb-5">Sisteme Giriş</h3>
                            </div>

                            <div class="col">
                                <div class="form-floating mb-3 ">
                                    <input type="email" class="form-control" id="floatingInput"
                                        placeholder="name@example.com">
                                    <label for="floatingInput"><i class="fa-solid fa-envelope me-2"></i>Email
                                        Adresi</label>
                                </div>
                            </div>

                            <div class="col">
                                <div class="form-floating mb-4">
                                    <input type="password" class="form-control" id="floatingPassword"
                                        placeholder="Password">
                                    <label for="floatingPassword"><i class="fa-solid fa-lock me-2"></i>Şifre</label>
                                </div>
                            </div>

                            <div class="col">
                               <a @click="auth" class="btn custom w-100 mb-5" href="#">Giriş Yap</a>
                            </div>

                            <div class="col">
                                <div class="logo">
                                    <img src="../../src/assets/img/robotum_logo.png" alt="" style="width: 235px;
                                    height: 51px;">
                                </div>
                            </div>
                        </div>
                    </form>
                </div>
                <div class="col-sm-12 col-md-12 col-lg-2 col-xl-2 col-xxl-2"></div>
            </div>



        </div>

    </div>
</template>

<script>


export default {
    data() {
        return {
            email: "",
        }
    },

  methods:{
        auth(){
            
            this.email = document.getElementById("floatingInput").value;
            switch(document.getElementById("floatingInput").value){
                case "admin":
                    this.$router.push ("/admin");
                    break;
                case "student":
                    this.$router.push ("/student");
                    break;
                default:
                    this.$router.push ("/teacher");
                    break;
            }
        }
    }

}
</script>

<style lang="scss" scoped>


$primary-color:#c13832;
$primary-color-v2:#c23129;
$primary-color-soft:#c139328e;

$darker-color:#b1352f;
$darker-color-soft:#b1362fa1;

$secondary-color:#d7d3c8;
$bubble-color:#d7d3c896;


$bc-mozilla: #c13832;
$bc-mozilla-1: #c13832;
$bc-mozilla-2: #d7d3c8;
$bc-mozilla-3: #4d4e53;


//wrapper colors

$wp-color-1: #b42922;
$wp-color-2: #c13832;
$wp-color-3: #c13832;
$wp-color-4: #c13832;



// X-Small devices (portrait phones, less than 576px)
// No media query for `xs` since this is the default in Bootstrap

// Small devices (landscape phones, 576px and up)
@media (min-width: 0px) {
    .hidden {

        display: block;

    }

    .sidebox{
        
        display: none;
    }

    .bubbles {

        display: none;

    }

}



@media (min-width: 576px) {
    .hidden {

        display: none;

    }

    .sidebox{
        
        display: none;
    }

    .bubbles {

        display: block;
        
    }

}

// Medium devices (tablets, 768px and up)
@media (min-width: 768px) {
    
    .sidebox{

        display: none;
    }

    .hidden {

        display: block;

    }

    .bubbles {

        display: none;
        
    }

}

// Large devices (desktops, 992px and up)
@media (min-width: 992px) {
    .hidden {

        display: none;

    }

    .sidebox{
        
        display: block;
    }

    .bubbles {

        display: block;
        
    }

}

// X-Large devices (large desktops, 1200px and up)
@media (min-width: 1200px) {
    .hidden {

        display: none;

    }

    .sidebox{
        
        display: block;
    }

    .bubbles {

        display: block;
        
    }
    
}

// XX-Large devices (larger desktops, 1400px and up)
@media (min-width: 1400px) {
    .hidden {

        display: none;

    }

    .sidebox{
        
        display: block;
    }

    .bubbles {

        display: block;
        
    }

}

.bubblesfull{
  position: absolute;
  width:100%;
  height: 100%;
  overflow:hidden;
  top:0;
  left:0;
  z-index: 99;
}
.bubbles{
    position: absolute;
    width:50%;
    height: 100%;
    overflow:hidden;
    top:0;
    left:0;
    z-index: 99;
  }
  .bubble{
    position: absolute;
    bottom:-500px;
    width:80px;
    height:80px;
    background: $bubble-color;
    border-radius:50%;
    opacity:0.5;
    animation: rise 10s infinite ease-in;
    z-index: 100;
  }
  .bubble:nth-child(1){
    width:100px;
    height:100px;
    left:10%;
    animation-duration:8s;
  }
  .bubble:nth-child(2){
    width:120px;
    height:120px;
    left:20%;
    animation-duration:5s;
    animation-delay:1s;
  }
  .bubble:nth-child(3){
    width:50px;
    height:50px;
    left:35%;
    animation-duration:7s;
    animation-delay:2s;
  }
  .bubble:nth-child(4){
    width:80px;
    height:80px;
    left:50%;
    animation-duration:11s;
    animation-delay:0s;
  }
  .bubble:nth-child(5){
    width:200px;
    height:200px;
    left:55%;
    animation-duration:6s;
    animation-delay:1s;
  }
  .bubble:nth-child(6){
    width:300px;
    height:300px;
    left:65%;
    animation-duration:8s;
    animation-delay:3s;
  }
  .bubble:nth-child(7){
    width:150px;
    height:150px;
    left:70%;
    animation-duration:12s;
    animation-delay:2s;
  }
  .bubble:nth-child(8){
    width:150px;
    height:150px;
    left:80%;
    animation-duration:6s;
    animation-delay:2s;
  }
  .bubble:nth-child(9){
    width:200px;
    height:200px;
    left:70%;
    animation-duration:5s;
    animation-delay:1s;
  }
  .bubble:nth-child(10){
    width:90px;
    height:90px;
    left:25%;
    animation-duration:10s;
    animation-delay:4s;
  }
  @keyframes rise{
    0%{
      bottom:-100px;
      transform:translateX(0);
    }
    50%{
      transform:translate(100px);
    }
    100%{
      bottom:1080px;
      transform:translateX(-200px);
    }
  }

body {
    margin: 0px !important;
    padding: 0px !important;
}

.row {
    margin: 0px !important;
    padding: 0px !important;
}

.col {
    margin: 0px !important;
    padding: 0px !important;
}

.sidebar {

    background-color: #fffefec5;
    height: 100vh;
    display: block;
}

.content {

    background-color: $primary-color;
    height: 100vh;
    z-index: 1000;
}

.hrbox {

    background-color: white;
    width: 70%;
    height: 3px;

    margin-bottom: 20px;

}

.title {

    font-size: 50pt;
    color: $primary-color;

}

.subtitle {

    font-size: 25pt;
    color: $primary-color-v2;

}

.description {

    color: $primary-color-v2;

}

a {

    color: $primary-color;
}

a:hover {

    color: $primary-color-soft;
}

.animation {

    position: relative;
    z-index: 999;
    background-color: white;
    width: 400px;
    height: 400px;

    text-align: start;
    border-radius: 20%;
    box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.075) inset, 0px 0px 20px $secondary-color;

    margin-top: 25%;
    margin-left: 27%;

}


.loginbox {
    position: relative;
    margin-top: 30% !important;
    z-index: 999;
}

.wrapper {

    background: linear-gradient(124deg, $primary-color, $darker-color, $primary-color, $darker-color, $primary-color);
    background-size: 1800% 1800%;
    -webkit-animation: rainbow 18s ease infinite;
    -z-animation: rainbow 18s ease infinite;
    -o-animation: rainbow 18s ease infinite;
    animation: rainbow 18s ease infinite;
}

@-webkit-keyframes rainbow {
    0% {
        background-position: 0% 82%
    }

    50% {
        background-position: 100% 19%
    }

    100% {
        background-position: 0% 82%
    }
}

@-moz-keyframes rainbow {
    0% {
        background-position: 0% 82%
    }

    50% {
        background-position: 100% 19%
    }

    100% {
        background-position: 0% 82%
    }
}

@-o-keyframes rainbow {
    0% {
        background-position: 0% 82%
    }

    50% {
        background-position: 100% 19%
    }

    100% {
        background-position: 0% 82%
    }
}

@keyframes rainbow {
    0% {
        background-position: 0% 82%
    }

    50% {
        background-position: 100% 19%
    }

    100% {
        background-position: 0% 82%
    }
}

.custom {

    border-color: $darker-color;
    color: white;
    background-color: $darker-color;
    box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.075) inset, 0px 0px 20px $darker-color-soft;

}

.custom:hover {

    border-style: solid;
    border-color: $primary-color;
    color: white;
    background-color: $primary-color-soft;

}

.customsm {

    border-style: solid;
    border-color: $primary-color-soft;
    color: white;
    background-color: $primary-color-v2;

}

.customsm:hover {

    border-color: $darker-color;
    color: white;
    background-color: $darker-color-soft;
    box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.075) inset, 0px 0px 12px $darker-color-soft;

}

.textshadow:hover {

    color: $secondary-color;
    text-shadow: 0 0 10px #35353579, 0 0 10px $primary-color-soft;
    font-size: 12pt;

}

.textshadowttl:hover {

    color: $secondary-color;
    text-shadow: 0 0 10px #35353579, 0 0 10px $primary-color-soft;
}

.form-control:hover {

    outline: 0 !important;

    -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 15px $darker-color-soft;
    border-color: $primary-color  !important;
    box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.075) inset, 0px 0px 15px $darker-color-soft;
    //background-color: $primary-theme-color-transparent  !important;



}

.form-control:focus {

    outline: 0 !important;

    -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, .075), 0 0 15px $darker-color-soft;
    border-color: $primary-color  !important;
    box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.075) inset, 0px 0px 15px $darker-color-soft;
    //background-color: $primary-theme-color-transparent  !important;

}

.spnr{
    color: $primary-color;
}

.logo{

    display: flex;
    justify-content: center;
}


</style>