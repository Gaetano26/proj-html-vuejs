<template>
  <div class="container">
    <div class="row row-cols-md-4 justify-content-center mt-5">
      <InfoComponent v-for="info in infos" :title="info.title"  :number="info.num"/>
    </div>

  </div>
</template>

<script>
import InfoComponent from '../components/InfoComponent.vue';
import { infos } from '../data/store';

export default {
  components: {
       InfoComponent,
  },
  data () {
    

    return {
      infos
    }
  }
}
</script>

<style lang="scss" scoped>

</style>