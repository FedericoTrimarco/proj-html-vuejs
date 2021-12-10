<template>
    <div class="section-one border">
        <!-- TOP -->
        <div class="section-one-top border">
            <div class="container border d-flex justify-content-between">
                <p><i class="far fa-map text-white"></i> <span class="text-white">International</span> International Shipping Service</p>
                <p><i class="far fa-clock text-white"></i> See our <span class="text-white">store hours</span> and service</p>
                <p><i class="fas fa-check text-white"></i> We price match to give you the <span class="text-white">best deals</span></p>
            </div>
        </div>
        <!-- CENTER -->
        <div class="section-one-center border d-flex align-items-center">
            <div class="container border text-white">
                <span class="fw-bold">FIND THE BEST ANIMAL SUPPLIES</span>
                <h1 class="my-4">We knows animals are a part of your family, let us help take care of them.</h1>
                <button class="btn pointer">Learn more about us</button>
            </div>
        </div>
        <!-- BOTTOM -->
        <div class="section-one-bottom border pt-2">
            <div class="container d-flex align-items-center border justify-content-center">
                <img src="../assets/food-transparent-5-200x112.png" alt="">
                <p class="text-white mx-2">Get $25 OFF your first purchase of our homemade pet food!</p>
                <a @click.prevent href="/">Visit the shop</a>
            </div>
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
    background-position: center;
    background-size: cover;
    span{
        letter-spacing: 3px;
    }
    h1{
        font-size: 50px;
        width: 40%;
        font-family: 'Domine', serif;
        text-shadow: 2px 2px 10px black;
    }
}
.section-one-bottom{
    background-image: url('../assets/bg-transparent-3.png');
    background-color: $heavyMetal;
    font-size: 20px;
    a{
        color: $naturalGrey;
    }
}

</style>