<template>
    <div class="section-two text-center border">
        <h1 class="mb-3">Browse by category</h1>
        <p class="fs-1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores laudantium, reprehenderit nam ad ipsam iste perferendis aut dolorum adipisci delectus veniam nulla.</p>
    </div>
</template>

<script>
export default {
    name: 'SectionTwo'
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