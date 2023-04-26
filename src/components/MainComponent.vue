<template>
  <div class="container">
    <div class="row row-cols-md-4 justify-content-center mt-5">
      <InfoComponent v-for="info in infos" :title="info.title"  :number="info.num"/>
    </div>
  </div>
  <div class="container marg">
    <div class="row">
      <AboutMeComponent />
    </div>
  </div>
  <div class="container marg2">
    <div class="row">
      <VideoComponent />
    </div>
  </div>
</template>

<script>
import InfoComponent from '../components/InfoComponent.vue';
import AboutMeComponent from '../components/AboutMeComponents.vue'
import VideoComponent from '../components/VideoComponent.vue'
import { infos } from '../data/store';

export default {
  name: 'MainComponent',
  components: {
       InfoComponent,
       AboutMeComponent,
       VideoComponent,
  },
  data () {
    

    return {
      infos
    }
  }
}
</script>

<style lang="scss" scoped>
 .marg {
  margin-top: 170px;
 }
 .marg2 {
  margin-top: 80px;
 }
</style>