<template>
  <div>
    <HeaderComponent />
    <MainComponent />
    <FooterComponent />

  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
import { testimonials } from './data/store';

export default {
  components: {
      HeaderComponent,
      MainComponent,
      FooterComponent,
  },
  data () {
    

    return {
      testimonials
    }
  }
}
</script>

<style lang="scss" scoped>

</style>