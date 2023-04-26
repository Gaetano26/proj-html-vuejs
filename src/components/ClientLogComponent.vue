<template>
    <div class="d-flex align-items-center">
       <img :src="image" :alt="image">
    </div>
</template>

<script>

import { clientLog } from '../data/store';
export default {
    props: ['image'],
    setup () {
        

        return {
            clientLog
        }
    }
}
</script>

<style lang="scss" scoped>

</style>