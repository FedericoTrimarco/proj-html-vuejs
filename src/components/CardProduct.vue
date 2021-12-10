<template>
    <div class="card border">
        <img :src="require(`../assets${src}`)" class="w-100">
        <h2 class="mt-2">{{title}}</h2>
        <span class="original-price">{{ originalPrice }}</span>
        <span class="current-price">{{ price }}</span>
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
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    h2{
        font-weight: normal;
    }
    span{
        color: $bayLeaf;
        font-size:x-large;
    }
    .original-price{
        text-decoration: line-through black;
        margin-right: 10px;
        font-size: initial;
    }

</style>