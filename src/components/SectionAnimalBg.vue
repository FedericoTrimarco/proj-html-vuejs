<template>
    <div class="section-animal border p-relative w-100">
        <div class="img h-100">
            <img :src="require(`../assets/${srcImg}`)" alt="" class="w-100 h-100">
        </div>
        <div class="info text-white border p-absolute centering">
            <span class="fw-bold">{{ spanText }}</span>
            <h1 class="my-4">{{ h1Text }}</h1>
            <button class="btn pointer">{{ btnText }}</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionAnimalBg',
    props:{
        srcImg: String,
        spanText: String,
        h1Text: String,
        btnText: String,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
.section-animal{
    height: 600px;
    img{
        filter: brightness(70%);
        object-fit: cover;
    }
    .info{
        text-align: center;
        span{
            letter-spacing: 3px;
        }
        h1{
            font-size: 50px;
            font-weight: normal;
            font-family: 'Domine', serif;
            text-shadow: 2px 2px 10px black;
        }

    }

}

</style>