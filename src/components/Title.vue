<template>
    <div class="title">
        <h1 class="mb-2">{{ title }}</h1>
        <p class="fs-1">{{ description }}</p>
    </div>
</template>

<script>
export default {
    name: 'Title',
    props:{
        title: String,
        description: String,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    
    h1{
        font-family: 'Domine', serif;
        color: $greenKelp;
        font-weight: normal;
    }
    p{
        color: $bayLeaf;
    }


</style>