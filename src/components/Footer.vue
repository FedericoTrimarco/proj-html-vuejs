<template>
    <footer class="border">
        <div class="container border d-flex flex-wrap justify-content-between py-6">
            <div class="company border">
                <img src="../assets/mobile-light-pet-logo-2x.png" alt="mobile-light-pet-logo" class="w-70 border">
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
                <h1>hreughreghuier</h1>
                <ul>
                    <li>bhjjgrehbe</li>
                    <li>bhjjgrehbe</li>
                    <li>bhjjgrehbe</li>
                    <li>bhjjgrehbe</li>
                </ul>
            </div>
            <div class="useful border">
                <h1>hreughreghuier</h1>
                <ul>
                    <li>bhjjgrehbe</li>
                    <li>bhjjgrehbe</li>
                    <li>bhjjgrehbe</li>
                    <li>bhjjgrehbe</li>
                </ul>
            </div>
            <div class="subscribe border d-flex flex-column">
                <h1>hreughreghuier</h1>
                <input type="email" placeholder="Insert your email...*" class="my-2">
                <button class="btn btn-green">gefygweyf</button>
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
        padding: 40px;
    }
    ul{
        list-style: none;
    }
    .subscribe{
        background-color: #264229;
        background-image:
            linear-gradient(rgba(0, 0, 0, 0) 40%, rgb(38, 66, 41) 60%), 
            url('../assets/bg-transparent-3.png')
        ;
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

</style>