<template>
    <div class="section-five container mb-6">
        <SectionAnimalBg
            srcImg="banner-3-2x-scaled.jpg"
            spanText="FIND THE BEST ANIMAL SUPPLIES"
            h1Text="New arrivals weekly"
            btnText="Learn more about us"
        />
    </div>
</template>

<script>
import SectionAnimalBg from '@/components/SectionAnimalBg.vue'
export default {
    name: 'SectionFive',
    components: {
        SectionAnimalBg,
    }

}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

</style>