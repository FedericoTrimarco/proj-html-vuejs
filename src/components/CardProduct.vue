<template>
    <div class="card border">
        <img :src="require(`../assets${src}`)" class="w-100">

        <div class="card-info">
            <h2 class="my-1">{{title}}</h2>
            <span v-if="originalPrice != null" class="original-price">{{ originalPrice }}</span>
            <span v-if="price != null" class="current-price">{{ price }}</span>
            <span v-else-if="date != null" class="date  ">{{ date }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardProduct',
    props:{
        src: String,
        title: String,
        price: String,
        originalPrice: String,
        date: String,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

    .card-info{
        padding: 0 10px;
        h2{
            font-weight: normal;
            word-spacing: 5px;
        }
        span{
            color: $bayLeaf;
            font-size: x-large;
        }
        .original-price{
            text-decoration: line-through black;
            margin-right: 10px;
            font-size: initial;
        }
        .date{
            color: #000;
            font-size: initial;
        }
    }

</style>