<template>
    <div class="col col-md-4 pt-3">
       <img class="img-fluid" :src="image" :alt="{image}">
       <div class="px-4 pt-3">
            <p class="fs-3 fw-bold">{{ price }}</p>
            <h3 class="fs-4">{{ name }}</h3>
            <div class="d-flex gap-4 mt-4">
                <p><i class="fa-regular fa-file"></i><span class="ps-2">{{ lessons }}</span></p>
                <p><i class="fa-regular fa-user"></i><span class="ps-2">{{ students }}</span></p>
            </div>
       </div>
      
    </div>
</template>

<script>
import { courses } from '../data/store';
export default {
    name: 'LatestCourses',
    props: ['image', 'price', 'name','lessons', 'students'],
    data () {
        

        return {
            courses
        }
    }
}
</script>

<style lang="scss" scoped>
   p {
    color:  #20ad96;
   }

   h3 {
    color: #3f3a64;
   }
</style>