<template>
    <div class="col col-md-4 pad">
        <h6>Book Store Online</h6>
        <h2 class="fs-1 mt-3">Be Alpha With <span>Wingman's Book</span></h2>
        <div class="mt-5">
            <p><i class="fa-solid fa-check"></i>  Help you understand your self better</p>
            <p><i class="fa-solid fa-check"></i>  Help you understand your self better</p>
            <p><i class="fa-solid fa-check"></i>  Help you understand your self better</p>
            <p><i class="fa-solid fa-check"></i>  Help you understand your self better</p>
            <button type="button" class="btn text-white mt-5 fw-bold">Get Free EBook</button>

        </div>
        
    </div>
    <div class="col col-md-8  d-flex mb-3">
        <BooksComponent v-for="book in books" :image="book.image" :name="book.name" :price="book.price"/>
    </div>
</template>

<script>
import BooksComponent from '../components/BooksComponent.vue';
import { books } from '../data/store';
export default {
    components: {
         BooksComponent,
    },
    setup () {
        

        return {
            books
        }
    }
}
</script>

<style lang="scss" scoped>

h6 {
    text-transform: uppercase;
}
span {
    color: #20ad96;
}

i {
    color: #20ad96;
}
.pad {
    padding-right: 100px;
}
button {
    background-color: #20ad96;
    padding: 13px 60px;
  }
</style>