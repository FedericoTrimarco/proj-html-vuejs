<template>
    <div class="fixed-items p-fixed">
        <div class="lello radius-10px mb-1">
            <i class="fab fa-vuejs"></i>
            <span>Demos</span>
        </div>
        <div class="lello radius-10px">
            <div class="price border p-relative">
                <div class="price-number  fw-bold">
                    <span class="p-absolute dollar fs-1">$</span>
                    <span class="fs-2">39</span>
                </div>
                <span>On Sale</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FixedWrapper'
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    .fixed-items{
        right: 20px;
        top: 180px;
        .lello{
            background-color: #fff;
            padding: 5px;
            width: 80px;
            height: 80px;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            box-shadow: 0px 0px 5px 0px;

            i{
                font-size: 40px;
                color: #33475b;
            }

            .price{
                .price-number{
                    color: #65bc7b;
                }
                .dollar{
                    top: 0;
                    left: 0;
                }
            }
        }
    }


</style>