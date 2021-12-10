<template>
    <div class="section-two text-center border">
        <Title title="Browse by category"
        description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores laudantium, reprehenderit nam ad ipsam iste perferendis aut dolorum adipisci delectus veniam nulla."/>
    </div>
</template>

<script>
import Title from '@/components/Title.vue'

export default {
    name: 'SectionTwo',
    components:{
        Title,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    .section-two{
        width: 30%;
        margin: 100px auto;
    }

</style>