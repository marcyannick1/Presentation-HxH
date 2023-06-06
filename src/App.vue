<template>
    <!-- <SideNav /> -->
    <Hero />
    <Presentation />
    <Divisor transforme="rotate(1deg) translate(-220px, -5vh)"/>
    <Personnages />
    <Divisor transforme="rotate(1deg) translate(-220px, -20vh)"/>
</template>

<script>
import SideNav from "./components/SideNav.vue";
import Hero from "./Hero.vue";
import Divisor from "./components/Divisor.vue";
import Presentation from "./Presentation.vue";
import Personnages from "./Personnages.vue";

export default {
    components: {
        SideNav,
        Hero,
        Divisor,
        Presentation,
        Personnages,
    },
};
</script>

<style scoped></style>
