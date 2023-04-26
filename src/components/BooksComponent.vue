<template>
    <div class="text-center">
        <img :src="image" :alt="image">
        <h5>{{ name }}</h5>
        <h6 class="fs-5">{{ price }}</h6>
        

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

</style>