<template>
    <footer class="border text-white">
        <!-- footer-top -->
        <div class="footer-top pb-4">
            <!-- Avada-pet-supplies / Shop-by-brand / Useful-link -->
            <div class="footer-top-top container border d-flex justify-content-between py-3 mb-5">
                <div v-for="(el, id) in linkFooterTop" :key="`link-footer-top${id}`" class="links border">
                    <img 
                        v-if="el.img != null"
                        :src="require(`@/assets/${el.img}`)"
                        :alt="el.img"
                        class="border w-100 mb-3"
                    >
                    <h2 v-else class="mb-3">{{ el.title }}</h2>
                    <ul class="list-none">
                        <li v-for="(el, id) in el.links" :key="`link-${id}`" class="mb-25px">
                            <a href="/" class="text-decoration-none text-white fs-1">{{el}}</a>
                        </li>
                    </ul>
                </div>
                <!-- subscribe -->
                <div class="subscribe border d-flex flex-column">
                    <div class="subscribe-content radius-10px">
                        <h2>Subscribe to your newsletter</h2>
                        <input type="email" placeholder="Insert your email...*" class=" w-100 my-2 fs-min radius-30px border-none">
                        <button class="btn btn-green w-100 pointer">Subscribe</button>
                    </div>
                </div>
            </div>
            <div class="footer-top-bottom border text-center">
                <!-- links-footer-top-bottom -->
                <ul class="footer-top-bottom-link d-flex justify-content-center mb-3 list-none">
                    <li v-for="(el, id) in linkFooterBottom1" :key="`link-bottom-${id}`" class="me-2">
                        <a href="/" @click.prevent class="text-decoration-none fs-1">{{ el }}</a>
                    </li>
                </ul>
                <!-- links-social -->
                <ul class="footer-top-bottom-social d-flex justify-content-center list-none">
                    <li v-for="(el, id) in linkFooterBottom2" :key="`link-social-${id}`" class="me-1">
                        <a href="/" @click.prevent class="text-white">
                            <i :class="el" class="text-decoration-none fs-1"></i>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <!-- footer-bottom -->
        <div class="footer-bottom text-center py-3">
            <p><i class="far fa-copyright"></i> Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</p>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    props:{
        linkFooterTop: Array,
        linkFooterBottom1: Array,
        linkFooterBottom2: Array,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    .footer-top{
        background-color: $greenKelp;
        .links, .subscribe{
            padding: 50px;
            width: calc(100% / 4);
        }
        .links:first-child{
            li{
                margin-bottom: 10px;
            }
        }
        .subscribe-content{
            background-color: #264229;
            background-image:
                linear-gradient(rgba(0, 0, 0, 0) 40%, rgb(38, 66, 41) 60%), 
                url('../assets/bg-transparent-3.png')
            ;
            padding: 50px;
        }
        input{
            background: $lightGray;
            padding: 15px;
            &::placeholder{
                color: #000;
            }
        }
        .footer-top-top{
            border-bottom: 1px solid $bandicoot;
        }
        .footer-top-bottom-link{
            a{  
                color: $naturalGrey;
                &:hover{
                    color: #fff;
                }
            }
        }
    }
    .footer-bottom{
        background-color: #000;
    }
</style>