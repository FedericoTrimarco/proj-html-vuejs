<template>
    <div class="section-six container border">
        <!-- info -->
        <div class="section-six-top border d-flex justify-content-between align-items-end mb-5">
            <div class="section-six-top-info">
                <span class="fw-bold ">All time best sellers</span>
                <p>Items everyone loves</p>
            </div>
            <button class="btn btn-green">View all products</button>
        </div>
        <!-- products -->
        <div class="section-six-bottom border">
            <!-- <CardProduct /> -->
            <ul class="list-none d-flex border justify-content-between text-center">
                <li v-for="(el, id) in mainArray" :key="`product-${id}`">
                    <CardProduct
                        :src="el.src"
                        :title="el.title"
                        :originalPrice="el.originalPrice"
                        :price="el.price"
                    />
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
import CardProduct from '@/components/CardProduct.vue'
export default {
    name:'SectionSix',
    props:{
        mainArray: Array,
    },
    components:{
        CardProduct,
    }
    
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
.section-six{
    .section-six-top-info{
        span{
            color: $bayLeaf;
            letter-spacing: 3px;
            font-size: 20px;

        }
        p{
            font-family: 'Domine', serif;
            font-size: 40px;
            margin-top: 30px
        }
    }
    .section-six-bottom{
        li{
            width: calc(100% / 4);
            padding: 0 20px;
        }
    }
}

</style>