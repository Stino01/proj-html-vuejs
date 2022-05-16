<template>
    <main>
        <hero-component/>
        <consult-component/>
        <about-component/>
    </main>
</template>

<script>
import HeroComponent from "./HeroComponent.vue"
import ConsultComponent from "./ConsultComponent.vue"
import AboutComponent from "./AboutComponents.vue"

export default {
    name: "MainApp",
    components: {
        HeroComponent,
        ConsultComponent,
        AboutComponent,
    }
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";
</style>