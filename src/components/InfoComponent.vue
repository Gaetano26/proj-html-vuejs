<template>
    <div class="col text-center pt-5" >
        <h2>{{ number }}</h2>
        <p>{{ title }}</p>
    </div>
</template>

<script>
import { infos } from '../data/store'
export default {
    name: 'InfoComponent',
    props: ['title', 'number'],
   
    

    data () {
        

        return {
            infos,
        }
    }
}
</script>

<style lang="scss" scoped>
  h2 {
    color:  #20ad96;
  }

</style>