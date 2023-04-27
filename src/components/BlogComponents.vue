<template>
    <div class="col">
        <img class="img-fluid" :src="image" :alt="image">
        <div class="mt-4">
            <i class="fa-regular fa-calendar"></i>
            <span class="ms-2">{{ data }}</span>
        </div>
        <h4 class="mt-3">{{ name }}</h4>
        <p class="mt-3">{{ text }}</p>

    </div>
</template>

<script>
import { text } from '@fortawesome/fontawesome-svg-core';


export default {
    name: 'BlogComponents',
    props: ['name', 'data', 'image', 'text'],
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>

</style>