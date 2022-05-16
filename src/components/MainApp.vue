<template>
    <main>
        <hero-component/>
    </main>
</template>

<script>
import HeroComponent from "./HeroComponent.vue"

export default {
    name: "MainApp",
    components: {
        HeroComponent
    }
}
</script>

<style lang="scss" scoped>
    @import "../style/vars.scss";
</style>