<script>
import MainSliderSection from "./MainSliderSection.vue";
import WelcomeSection from "./WelcomeSection.vue";
import ServiceSection from "./ServiceSection.vue";

export default {
    components: {
        MainSliderSection,
        WelcomeSection,
        ServiceSection
    }
}
</script>

<template>
    <MainSliderSection></MainSliderSection>

    <WelcomeSection></WelcomeSection>

    <ServiceSection></ServiceSection>
    
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;
</style>