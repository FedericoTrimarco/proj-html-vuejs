<template>
    <!-- FOODS -->
    <div class="section-four container d-flex border">
        <div v-for="(el, id) in arrayElements" :key="`food-${id}`" class="border card text-center" >
            <div class="food py-6">
                <h1 class="text-white">{{ el.title }}</h1>
                <p class="mt-3 fw-bold">{{ el.description }}</p>
                <div class="food-img">
                    <img :src="require(`../assets${el.srcFood}`)" :alt="el.title" class="w-70">
                </div>
                <button class="btn btn-green pointer">{{ el.btnText }}</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionFour',
    props: {
        arrayElements: Array,
    },
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    .section-four{
        .card{
            width: calc(100% / 3);
            padding: 10px;
            .food{
                background-color: $heavyMetal;
                background-image:
                                    linear-gradient(rgba(0, 0, 0, 0) 20%, rgb(30, 48, 32) 80%), 
                                    url('../assets/bg-transparent-3.png')
                                ;
                transition: transform .5s;
                &:hover{
                    transform: scale(1.05)
                }
                h1{
                    font-family: 'Domine', serif;
                    letter-spacing: 3px;
                }
                p{
                    color: $bayLeaf;
                    font-size: 20px;
                    letter-spacing: 2px;
                }
            }
        }
    }
</style>