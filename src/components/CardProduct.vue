<template>
    <div class="card border">
        <div class="img p-relative border pointer">
            <img :src="require(`../assets${src}`)" class="w-100 h-100 border">
            <div v-if="hover != false" class="hover-item p-absolute centering border w-100 h-100 d-flex justify-content-center align-items-center">
                <div v-if="check != false" class="border text-white">
                    <i class="far fa-check-square fs-2 border check mb-1"></i>
                    <p>VIEW CART</p>
                </div>
                <div v-else class="text-center text-white">
                    <h1 class="fw-normal border px-20px">{{title}}</h1>
                    <span>Tips & Tricks</span>
                </div>
            </div>
        </div>

        <div class="card-info">
            <h2 class="my-1">{{title}}</h2>
            <span v-if="originalPrice != null" class="original-price">{{ originalPrice }}</span>
            <span v-if="price != null" class="current-price">
                {{ price }}
                <span v-if="secondPrice != null" class="dash"> - </span>
                {{secondPrice}}
            </span>
            <span v-else-if="date != null" class="date">{{ date }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardProduct',
    props:{
        src: String,
        title: String,
        price: String,
        secondPrice: String,
        originalPrice: String,
        date: String,
        hover: Boolean,
        check: Boolean,
    },
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    
    .hover-item{
        transition: all 0.6s;
        opacity: 0;
        &:hover{
            background-color: rgba(164, 95, 66, 0.5);
            opacity: 1;
        }
        .check{
            padding: 20px;
            border-radius: 60px;
            background-color: rgb(0, 0, 0, .7);
        }
    }

    .card-info{
        padding: 0 10px;
        h2{
            font-weight: normal;
            word-spacing: 5px;
        }
        span{
            color: $bayLeaf;
            font-size: x-large;
        }
        .original-price{
            text-decoration: line-through black;
            margin-right: 10px;
            font-size: initial;
        }
        .date{
            color: #000;
            font-size: initial;
        }
        .dash{
            color: #000;
        }
    }

</style>