<template>
    <div class="text-center bcs">
        <div>
            <img :src="image" :alt="image">
            <h5>{{ name }}</h5>
            <h6 class="fs-5">{{ price }}</h6>
        </div>
        <div class="gap-2 search">
            <div class="cont-icon d-flex align-items-center justify-content-center">
                <i class="fa-solid fa-magnifying-glass"></i>
            </div>
            <div class="cont-icon d-flex align-items-center justify-content-center">
                <i class="fa-solid fa-cart-shopping"></i>
            </div>
            <div class="cont-icon d-flex align-items-center justify-content-center">
                <i class="fa-regular fa-heart"></i>
            </div>
            <div class="cont-icon d-flex align-items-center justify-content-center">
                <i class="fa-solid fa-arrow-up-wide-short"></i>
            </div>
        </div>
        
        

    </div>
</template>

<script>
import { books } from '../data/store';
export default {
    props: ['image', 'price', 'name',],
    data () {
        

        return {
            books
        }
    }
}
</script>

<style lang="scss" scoped>
h5 {
    color: #3f3a64;
}
 h6 {
    color:  #20ad96;
 }

.cont-icon {
    width: 45px;
    height: 45px;
    border-radius: 50%;
    background-color: white;
    
}

.bcs {
    position: relative;
      
    .search{
        position: absolute;
        top: 90px;
        right: 55px;
        display: none;
    }

}
.bcs:hover {

   .search {
    display: flex;
    flex-direction: column;
   }

}

</style>