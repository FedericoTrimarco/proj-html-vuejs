<template>
    <div class="section-one border">
        <div class="section-one-top border">
            <div class="container border d-flex justify-content-between">
                <p><i class="far fa-map text-white"></i> <span class="text-white">International</span> International Shipping Service</p>
                <p><i class="far fa-clock text-white"></i> See our <span class="text-white">store hours</span> and service</p>
                <p><i class="fas fa-check text-white"></i> We price match to give you the <span class="text-white">best deals</span></p>
            </div>
        </div>
        <div class="section-one-center border d-flex align-items-center">
            <div class="container border text-white">
                <span>FIND THE BEST ANIMAL SUPPLIES</span>
                <h1 class="my-4">We knows animals are a part of your family, let us help take care of them.</h1>
                <button class="btn pointer">Learn more about us</button>
            </div>

        </div>
        <div class="section-one-bottom border">
            <div class="container"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionOne',
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

.section-one-top{
    background-image: url('../assets/bg-transparent-3.png');
    background-color: $heavyMetal;
    .container{
        padding: 20px 100px;
        p{
            color: $westar; 
        }
    }
}
.section-one-center{
    height: 1000px;
    background-image: url('../assets/banner-5-2x-scaled.jpg');
    background-size: cover;
    span{
        letter-spacing: 3px;
    }
    h1{
        font-size: 50px;
        width: 27%;
        font-family: 'Domine', serif;
        text-shadow: 2px 2px 10px black;
    }
}
.section-one-bottom{
    background-image: url('../assets/bg-transparent-3.png');
    background-color: $heavyMetal;
}

</style>