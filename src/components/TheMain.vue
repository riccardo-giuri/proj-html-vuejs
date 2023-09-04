<script>
import MainSliderSection from "./MainSliderSection.vue";
import WelcomeSection from "./WelcomeSection.vue";

export default {
    components: {
        MainSliderSection,
        WelcomeSection
    }
}
</script>

<template>
    <MainSliderSection></MainSliderSection>

    <WelcomeSection></WelcomeSection>
    
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;
</style>