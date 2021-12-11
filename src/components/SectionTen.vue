<template>
    <div class="popular-accessories border d-flex">
        <SectionAnimalBg
            srcImg="banner-8-2x.jpg"
            spanText="FIND THE BEST ANIMAL SUPPLIES"
            h1Text="Popular accessories"
            btnText="View all toys accessories"
        />
        <SectionAnimalBg
            srcImg="banner-9-2x.jpg"
            spanText="FIND THE BEST FOOD"
            h1Text="New food arrival"
            btnText="View all food products"
        />
    </div>
</template>

<script>
import SectionAnimalBg from '@/components/SectionAnimalBg.vue'
export default {
    name:'SectionTen',
    components: {
        SectionAnimalBg,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

</style>