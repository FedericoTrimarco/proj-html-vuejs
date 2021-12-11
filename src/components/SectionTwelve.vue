<template>
    <div class="section-twelve border mb-8">
        <div class="container border text-center">
            <!-- title -->
            <Title title="New products arrival" description="latest product"/>
            <!-- new-articles -->
            <div class="articles">
                <ul class="list-none d-flex flex-wrap border text-center">
                    <li v-for="(el, id) in mainArray" :key="`product-${id}`" class="mb-2">
                        <CardProduct
                            :src="el.src"
                            :title="el.title"
                            :originalPrice="el.originalPrice"
                            :price="el.price"
                            :secondPrice="el.secondPrice"
                        />
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
import Title from '@/components/Title.vue'
import CardProduct from '@/components/CardProduct.vue'
export default {
    name: 'SectionTwelve',
    components:{
        Title,
        CardProduct,
    },
    props:{
        mainArray: Array,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

    li{
        width: calc(100% / 3);
        padding: 10px;
    }

</style>