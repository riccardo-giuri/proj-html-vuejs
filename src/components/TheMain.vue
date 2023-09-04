<script>
import MainSliderSection from "./MainSliderSection.vue";
import WelcomeSection from "./WelcomeSection.vue";
import ServiceSection from "./ServiceSection.vue";
import ChooseUsSection from "./ChooseUsSection.vue";
import ReviewSection from "./ReviewSection.vue";
import TheFooter from "./TheFooter.vue";

export default {
    components: {
        MainSliderSection,
        WelcomeSection,
        ServiceSection,
        ChooseUsSection,
        ReviewSection,
        TheFooter
    }
}
</script>

<template>
    <MainSliderSection></MainSliderSection>

    <WelcomeSection></WelcomeSection>

    <ServiceSection></ServiceSection>

    <ChooseUsSection></ChooseUsSection>

    <ReviewSection></ReviewSection>

    <TheFooter></TheFooter>
</template>

<style lang="scss" scoped>
    @use "../sass/partials/variables" as *;
</style>