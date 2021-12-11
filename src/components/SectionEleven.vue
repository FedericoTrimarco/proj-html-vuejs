<template>
    <div class="section-eleven border py-6 mb-6">
        <div class="container border">
            <ul class="list-none d-flex justify-content-between text-center">
                <li v-for="(el, id) in mainArray" :key="`icon-${id}`">
                    <i :class="el.iconClass" class="text-white fs-3 mb-2"></i>
                    <p class="fs-1">{{ el.iconText }}</p>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionEleven',
    props:{
        mainArray: Array,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    .section-eleven{
        background-color: $heavyMetal;
        background-image:
            linear-gradient(rgba(0, 0, 0, 0) 30%, rgb(30, 48, 32) 70%), 
            url('../assets/bg-transparent-3.png')
        ;
        p{
            color: $westar;
        }
    }

</style>