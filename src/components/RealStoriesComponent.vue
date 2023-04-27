<template>
    <div class="col">
        <div class="text-center mt-5 pt-5 cont-real">
            <h6 class="real">Real Stories</h6>
            <p class="mt-5">{{ testimonials[activeIndex].text }}</p>
            <img class="mt-3" :src="testimonials[activeIndex].image" :alt="testimonials[activeIndex].image">
            <h6 class="mt-3">{{ testimonials[activeIndex].name }}</h6>
            <p>{{ testimonials[activeIndex].role }}</p>
            <div class="d-flex flex-column align-items-center text-center pt-1 gap-1 cont-btn ">
                
                <img src="../assets/icon/icons8-freccia-comprimi-16.png" alt="" @click="Next">
                <p class="m-0">{{ testimonials[activeIndex].number}}/4</p>
                <img src="../assets/icon/icons8-freccia-espandi-16.png" alt="" @click="Prev">
                
                
            </div>
        </div>
        

    </div>
    <div class="col">
        <img class="img-fluid" src="/public/images/home-movation-testimonial-image-768x562.jpg" alt="">
    </div>
</template>

<script>
import { testimonials } from '../data/store';
export default{
    data () {
        

        return {
            testimonials,
            activeIndex: 0,
        }
    },
    methods: {
        Prev() {
           if( this.activeIndex === 0){
            this.activeIndex = testimonials.length -1;
           } else{
              this.activeIndex--;
           } 
        },
        Next() {
            if( this.activeIndex === testimonials.length -1){
                this.activeIndex = 0
            }else {
               this.activeIndex++;
            }
    }
    }
      
}
</script>

<style lang="scss" scoped>

 .cont-real {
    padding: 0 220px;
    position: relative;
    img {
        width: 70px;
        height: 70px;
        border-radius: 50%;
    }
 }

 button {
    border : none;
 }


 .real {
    color:  #20ad96
 }

 .cont-btn {
     width: 60px;
     height: 60px;
     background-color: white;
     border-radius: 50%;
     position: absolute;
     top:180px;
     right: -55px;
     
     img {
        width: 10px;
        height: 10px;
     }
 }

</style>