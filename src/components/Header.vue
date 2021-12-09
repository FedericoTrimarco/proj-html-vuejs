<template>
    <header class="border">
        <!-- header-top -->
        <div class="header-top container border d-flex align-items-center justify-content-between py-2">
            <!-- logo -->
            <div class="logo">
                <img src="../assets/dark-pet-logo.png" alt="logo">
            </div>
            <!-- input -->
            <div class="input">
                <i class="fas fa-search me-1"></i>
                <input type="text" placeholder="search...">
            </div>
            <!-- Questions -->
            <span><strong>Questions?</strong> Call us: 1.800.123.4567</span>
            <!-- icons -->
            <div class="icons">
                <i class="fas fa-archive me-1"></i>
                <i class="far fa-user"></i>
            </div>
        </div>
        <nav class="header-bottom container">
            <ul class="d-flex list-none border justify-content-center">
                <li class="me-3">
                    <a href="/" class="text-decoration-none">fsefwfewe <i class="fas fa-angle-down ms-1"></i></a>
                </li>
                <li class="me-3">
                    <a href="/" class="text-decoration-none">fsefwfewe <i class="fas fa-angle-down ms-1"></i></a>
                </li>
                <li class="me-3">
                    <a href="/" class="text-decoration-none">fsefwfewe <i class="fas fa-angle-down ms-1"></i></a>
                </li>
                <li class="me-3">
                    <a href="/" class="text-decoration-none">fsefwfewe <i class="fas fa-angle-down ms-1"></i></a>
                </li>
                <li class="me-3">
                    <a href="/" class="text-decoration-none">fsefwfewe <i class="fas fa-angle-down ms-1"></i></a>
                </li>
                
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
name: 'Header',
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
    .header-top{
        div,span{
            border: 1px solid blue;
        }
        .input{
            background: #f3f4f3;
            padding: 15px;
            border-radius: 30px;
            width: 500px;
            input{
                border: none;
                background: transparent;
            }
        }
    }
    .header-bottom{
        li{
            a{
                color: #9b9b9b;
            }
            i{
                font-size: 10px;
            }

        }
    }
</style>