<template>
    <footer class="border text-white py-6">
        <div class="footer-top container border d-flex justify-content-between py-3">
            <div class="company border">
                <img src="../assets/mobile-light-pet-logo-2x.png" alt="" class="border w-100 mb-3">
                <ul class="list-none">
                    <li>
                        <a href="/">1234 Avada Avenue Avadaville</a>
                    </li>
                    <li>
                        <a href="/">info@your-company.com</a>
                    </li>
                    <li>
                        <a href="/">Call us: (1) 234 5678</a>
                    </li>
                </ul>
            </div>
            <div class="shop border">
                <h2>Shop by brand</h2>
                <ul>
                    <li>
                        <a href="/">Bed</a>
                    </li>
                    <li>
                        <a href="/">Food</a>
                    </li>
                    <li>
                        <a href="/">Toys</a>
                    </li>
                    <li>
                        <a href="/">Transport</a>
                    </li>
                </ul>
            </div>
            <div class="useful border">
                <h2>Useful links</h2>
                <ul>
                    <li>
                        <a href="/">My account</a>
                    </li>
                    <li>
                        <a href="/">Orders</a>
                    </li>
                    <li>
                        <a href="/">Checkout</a>
                    </li>
                    <li>
                        <a href="/">Cart</a>
                    </li>
                </ul>
            </div>
            <div class="subscribe border d-flex flex-column">
                <div class="lello">
                    <h2>Subscribe to your newsletter</h2>
                    <input type="email" placeholder="Insert your email...*" class="my-2">
                    <button class="btn btn-green w-100">Subscribe</button>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    footer{
        background-color: $greenKelp;
    }
    .company, .shop, .useful, .subscribe{
        padding: 70px;
        width: calc(100% / 4);
    }
    h2{
        margin-bottom: 30px;
    }
    .company{
        li{
            margin-bottom: 10px;
        }
    }
    ul{
        list-style: none;
        li{
            margin-bottom: 25px;
            a{
                text-decoration: none;
                color: #fff;
                font-size: 20px;
            }
        }
    }
    .lello{
        background-color: #264229;
        background-image:
            linear-gradient(rgba(0, 0, 0, 0) 40%, rgb(38, 66, 41) 60%), 
            url('../assets/bg-transparent-3.png')
        ;
        padding: 50px;
        border-radius: 10px;
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
    .footer-top{
        border-bottom: 1px solid $bandicoot;
    }

</style>