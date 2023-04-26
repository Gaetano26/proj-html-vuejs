<template>
    <div class="col">
        <div class="cont-img">
            <img class="img1" src="../assets/icon/home-movation-video-poster-670x450.jpg" alt="">
            <img class="img2" src="../assets/icon/icon-youtube-play.png" alt="">
        </div>

    </div>
    <div class="col ps-5 pt-5">
        <p class="fs-3">"Every morning you have two choices: Continue to sleep with your dreams or wake up and chase them."</p>
        <img class="mt-5" src="../assets/icon/home-movation-shape-01.png" alt="">
        <h3 class="mt-4">Kaixa Stark</h3>
        <p>Wingman</p>
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
   .cont-img {
       width: 750px;
       position: relative;
       .img1 {
        width: 750px;
       }
       .img2 {
         position: absolute;
         top:230px;
         left:345px;
    

       }
   }

   p {
    padding-right: 100px;
   }

   h3{
    color: #3f3a64;
   }

</style>