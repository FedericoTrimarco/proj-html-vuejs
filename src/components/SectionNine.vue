<template>
    <div class="container border text-center mb-6">
        <!-- title -->
        <Title title="Get the best tip & tricks"
        description="Recent articles"/>
        <!-- list-articles -->
        <div class="tricks mt-3">
            <ul class="list-none d-flex border justify-content-between text-center">
                <li v-for="(el, id) in mainArray" :key="`product-${id}`">
                    <CardProduct
                        :src="el.src"
                        :title="el.title"
                        :date="el.date"
                    />
                </li>
            </ul>
        </div>
        <!-- button -->
        <button class="btn btn-green pointer mt-4">Read all articles</button>
    </div>
</template>

<script>
import Title from '@/components/Title.vue'
import CardProduct from '@/components/CardProduct.vue'

export default {
    name: 'SectionNine',
    components:{
        Title,
        CardProduct,
    },
    props: {
        mainArray: Array,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

    li{
        text-align: start;
        width: calc(100% / 4);
        margin-right: 50px;
        &:last-child{
           margin-right: 0;
        }
        
    }


</style>