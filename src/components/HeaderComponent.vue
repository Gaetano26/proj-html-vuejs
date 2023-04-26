<template>
    <header>
       <div class="container">
        <div class="row p-0">
            <NavBarComponent />

        </div>
       </div>

    </header>
</template>

<script>
import NavBarComponent from '../components/NavbarComponent.vue'

export default {
    name: 'HeaderComponent',
    components: {
        NavBarComponent,
    },
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>

</style>