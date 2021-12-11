<template>
    <div class="container border p-relative">
        <div class="newsletter-info border">
            <h1>Join our newsletters</h1>
            <p class="my-3">Volutpat vel turpis nulla lorem sed semper, Aliquam sagittis sem libero viverra vehicula nullam ut nisl.</p>
            
            <div class="send-email d-flex">
                <input type="email" placeholder="Insert your email...*" class="flex-grow-1 me-2">
                <button class="btn btn-green">Subscribe</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionEight'
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';

    .container{
        box-shadow: 0px 0px 11px 0px;
        background-image: url('../assets/banner-7-2x-scaled.jpg');
        background-size: cover;
        bottom: 100px;
        padding: 200px 150px;
        .newsletter-info{
            width: 50%;
            h1{
                font-family: 'Domine', serif;
                font-weight: normal;
                font-size: 50px;
            }
            p{
                font-size: 20px;
                line-height: 30px;
                word-spacing: 5px
            }
            input{
                background: $lightGray;
                border-radius: 30px;
                border: none;
                padding: 15px;
                font-size: 16px;
                &::placeholder{
                    color: #000;
                }
            }
        }
    }
</style>