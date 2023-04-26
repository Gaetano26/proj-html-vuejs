<template>
    <div class="col pt-5 mt-5 ">
      <div class="title">
        <h6>I'm Wingam</h6>
        <h1>Peace on Heart A Wonderful Wish But No Way</h1>
        <p class="mt-4">Success isn't overnight. It'when everyday you get a little better than the day before. It all adds up.</p>
        <button type="button" class="btn text-center text-white fw-bold mt-3">Get Started for free <i class="fa-solid fa-arrow-right ps-2"></i></button>
      </div>
        

    </div>
    <div class="col pt-3 d-flex justify-content-between">
      <div class="cont-img">
         <img class="img-fluid" src="../assets/icon/home-movation-hero-image.png" alt="image-hero">
      </div>
      <div class="d-flex flex-column align-items-center gap-2 mt-5 bg-white log">
        <a href=""><img class="dim" src="../assets/icon/Immagine 2023-04-26 144613.png" alt=""></a>
        <a href=""><img class="dim2" src="../assets/icon/icona.png" alt=""></a>
        <a href=""><i class="fa-solid fa-book"></i></a>
        <a href=""><i class="fa-solid fa-cart-shopping"></i></a>
       
      </div>
     

    </div>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>
  h6 {
    text-transform: uppercase;
  }
  .title {
    padding-left: 110px;
    padding-right: 200px;
  }
  h1 {
    font-size: 55px;
  }
  p {
    color: #20ad96;
  }

  button {
    background-color: #20ad96;
    padding: 13px 100px;
  }

  button:Hover {
    background-color: #3f3a64;
  }
  .dim {
    width: 20px;
    height: 20px;
  }
  .dim2 {
    width: 30px;
    height: 35px;
  }

  a {
    color: black;
  }
  
  .log {
    height: 135px;
  }
  .cont-img{
    background-image: url('../assets/icon/home-movation-shape-face-600x534.png');
  }
</style>