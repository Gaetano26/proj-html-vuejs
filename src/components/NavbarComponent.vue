<template>
    <div class="col co">
        <div class="d-flex pt-3 ps-3">
            <img src="../assets/icon/dark-logo.png" alt="logo">
        </div>
    </div>
    <div class="col d-flex pt-3 gap-3 align-items-center">
        <div class="dropdown">
            <button class="dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
               Home
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul> 
        </div>
        <div class="dropdown">
            <button class="dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                Pages
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul> 
        </div>
        <div class="dropdown">
            <button class="dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                Courses
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul> 
        </div>
        <div class="dropdown">
            <button class="dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                Features
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul> 
        </div>
        <div class="dropdown">
            <button class="dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                Blog
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul> 
        </div>
        <div class="dropdown">
            <button class="dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                Shop
            </button>
            <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul> 
        </div>
        
    </div>
    <div class="col d-flex gap-3 pt-3 align-items-center justify-content-center">
        <a href=""><img src="../assets/icon/twitter.svg" alt=""></a>
        <a href=""><img src="../assets/icon/facebook-f.svg" alt=""></a>
        <a href=""><img src="../assets/icon/instagram.svg" alt=""></a>
        <a href=""><img src="../assets/icon/linkedin.svg" alt=""></a>
        
    </div>
    
</template>

<script>
    export default {
        name:'NavBarComponent'
        
    }
</script>

<style lang="scss" scoped>
   img {
    width: 150px;
    height: 30px;
   }
   
   button {
    border: none;
    color: #3f3a64;
    background-color: transparent;
   }

   button:hover {
    border-bottom: 2px solid #20ad96;
    color: #20ad96;

    
   }
   
   i {
    color:  blacks;
   }
   a {
    img{
        width: 20px;
        height: 20px;
    }
   }
   .dropdown:hover {
     .dropdown-menu {
        display: block;
     }
   }
</style>