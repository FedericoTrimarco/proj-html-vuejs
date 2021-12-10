<template>
    <div class="section-two text-center border">
        <h1 class="mb-3">{{ title }}</h1>
        <p class="fs-1">{{ description }}</p>
    </div>
</template>

<script>
export default {
    name: 'SectionTwo',
    props:{
        title: String,
        description: String,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
.section-two{
    width: 30%;
    margin: 100px auto;
    h1{
        font-family: 'Domine', serif;
        color: $heavyMetal;
    }
}

</style>