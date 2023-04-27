<template>
 <footer class="marg">
     <div class="container">
        <div class="row">
            <div class="col col-md-6 py-5 mt-4">
               <h5 class="text-white">Address</h5>
               <p>382 NE 191st St # 87349 Miami, FL 31179-3899</p>
               <p>+1(305)549-9909(9am - 5pm EST, Monday-Friday)</p>
               <p>support@maxcoach.com</p>
               <div class="mt-4 d-flex gap-4">
                <a href=""><i class="fa-brands fa-square-facebook fs-4 "></i></a>
                <a href=""><i class="fa-brands fa-twitter fs-4 ms-3"></i></a>
                <a href=""><i class="fa-brands fa-instagram fs-4 ms-3"></i></a>
                <a href=""><i class="fa-brands fa-linkedin fs-4 ms-3"></i></a>
               </div>
            </div>
            <div class="col col-md-1 py-5 mt-4">
                <h5 class="text-white">Explore</h5>
                <p>Start Here</p>
                <p>Blog</p>   
                 <p>About us</p>  
                       
            </div>
            <div class="col col-md-2 py-5 mt-5 ps-5">
                 <p class="mt-2">Success story</p>
                 <p>Courses</p>
                 <p>Contact us</p> 
            </div>
            <div class="col col-md-3 py-5 mt-4">
                <h5 class="text-white">Information</h5>
                <p>Membership</p>
                <p>Purchase guide</p>
                <p>Privacy policity</p>
                <p>Terms of service</p>
            </div>
        </div>
        <div class="row marg2">
            <div class="col col-md-11">
                <p class="fw-bold text-center ms-5"><i class="fa-regular fa-copyright"></i> 2020 Maxcoach. All Rights Reserved</p>
                
            </div>
            <div class="col col-md-1 text-end ps-5 py-3">
                <div class="cont-arr d-flex align-items-center justify-content-center ms-5"> 
                 <a href=""><i class="fa-solid fa-arrow-up text-white fs-3"></i></a>
                </div>
            </div>
        
        </div>
    </div>
 </footer>
</template>

<script>

export default {
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>
footer {
    width: 100%;
    background-color: #171621;
}
.marg {
  margin-top: 170px;
 }

 .marg2 {
  margin-top: 50px;
 }

 p {
    color: grey;
    
 }

 a {
    text-decoration: none;
    color: grey;
 }

 .cont-arr {
    background-color:  #20ad96;
    width: 70px;
    height: 70px;
    border-radius: 50%;
 } 



</style>