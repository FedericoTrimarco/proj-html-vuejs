<template>
    <header class="border">
        <!-- header-top -->
        <div class="header-top ">
            <div class="header-top-content container border d-flex align-items-center justify-content-between py-2">
                <!-- logo -->
                <div class="logo">
                    <img src="../assets/dark-pet-logo.png" alt="logo">
                </div>
                <!-- input -->
                <div class="input">
                    <i class="fas fa-search me-1"></i>
                    <input type="text" placeholder="search..." class="fs-1 outline-none">
                </div>
                <!-- Questions -->
                <span class="text-end"><strong>Questions?</strong> Call us: 1.800.123.4567</span>
                <!-- icons -->
                <div class="icons text-end">
                    <i class="fas fa-archive me-1"></i>
                    <i class="far fa-user"></i>
                </div>
            </div>

        </div>
        <!-- Navbar links -->
        <nav class="header-bottom container">
            <ul class="d-flex list-none border justify-content-center">
                <li v-for="(link, id) in links" :key="id" class="me-3">
                    <a @click.prevent href="/" class="text-decoration-none fw-bold">{{ link }} <i class="fas fa-angle-down ms-1"></i></a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Header',
    props:{
        links: Array,
    }
}
    
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    .header-top{
        border-bottom: 1px solid $lightGray;
        .header-top-content{
            div,span{
                 width: calc(100% / 4);
                 padding: 0 15px;
            }
        }
        .input{
            background: $lightGray;
            border-radius: 30px;
            color: $naturalGrey;
            input{
                border: none;
                background: transparent;
                padding: 15px;
            }
        }
    }
    .header-bottom{
        padding: 15px;
        li{
            a{
                color: $naturalGrey;
                &:hover, &:focus{
                    color: #000;
                }
            }
            i{
                font-size: 10px;
            }

        }
    }
</style>