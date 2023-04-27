<template>
    <header>
       <div class="container">
            <div class="row p-0">
                <NavBarComponent />
            </div>
       </div>
       <div class="container-fluid bck">
                <div class="row mt-5">
                    <HeroComponent />

                </div>
        </div>

    </header>
</template>

<script>

import NavBarComponent from '../components/NavbarComponent.vue'
import HeroComponent from '../components/HeroComponent.vue'
export default {
    name: 'HeaderComponent',
    components: {
        NavBarComponent,
        HeroComponent,
        
    },
    data () {
        

        return {
            
        }
    }
}
</script>

<style lang="scss" scoped>
 header {
    background-image: url('../assets/icon/background-pattern-wavify.png');
    background-color: #f5f1ed;
 }
</style>