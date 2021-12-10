<template>
    <!-- SHOP -->
    <div class="section-three container border">
        <ul class="list-none d-flex border justify-content-between text-center">
            <li v-for="(el, id) in mainArray" :key="`image-${id}`">
                <CardProduct :src="el.src" :title="el.title"/>
            </li>
        </ul>
    </div>
</template>

<script>
import CardProduct from '@/components/CardProduct.vue'
export default {
    name: 'SectionThree',
    components:{
        CardProduct,
    },
    props: {
        mainArray: Array,
    },
    
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

.section-three{
    margin-bottom: 100px;
    li{
        width: calc(100% / 4);
        padding: 10px;
    }
}

</style>