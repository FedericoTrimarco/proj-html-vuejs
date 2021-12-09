<template>
    <div class="section-three container border">
        <ul class="list-none d-flex border justify-content-between text-center">
            <li v-for="(el, id) in mainArray" :key="`image-${id}`">
                <div class="card">
                    <img :src="require(`../assets${el.src}`)" class="w-100">
                    <h2 class="mt-3">{{el.title}}</h2>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'SectionThree',
    props: {
        mainArray: Array,
    }
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