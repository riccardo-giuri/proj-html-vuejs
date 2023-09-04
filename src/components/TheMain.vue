<script>
import MainSliderSection from "./MainSliderSection.vue";
import WelcomeSection from "./WelcomeSection.vue";
import ServiceSection from "./ServiceSection.vue";
import ChooseUsSection from "./ChooseUsSection.vue";

export default {
    components: {
        MainSliderSection,
        WelcomeSection,
        ServiceSection,
        ChooseUsSection
    }
}
</script>

<template>
    <MainSliderSection></MainSliderSection>

    <WelcomeSection></WelcomeSection>

    <ServiceSection></ServiceSection>

    <ChooseUsSection></ChooseUsSection>
    
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;
</style>