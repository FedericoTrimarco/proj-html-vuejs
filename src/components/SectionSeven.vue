<template>
    <div class="section-seven border text-white">
        <div class="container border text-center">
            <h1>Users testimonials</h1>
            <div class="users border mt-6">
                <ul class="border d-flex list-none">
                    <li class="border" v-for="(user, id) in mainArray" :key="`user-${id}`">
                        <img :src="require(`../assets${user.userSrc}`)" :alt="user.name">
                        <p class="my-2">{{ user.info }}</p>
                        <span>{{ user.name }}</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectiionSeven',
    props: {
        mainArray: Array,
    }
}
</script>

<style scoped lang="scss">
@import '@/Style/utilities.scss';
@import '@/Style/variables.scss';
    .section-seven{
        padding-top: 150px;
        padding-bottom: 300px;
        background-color: $heavyMetal;
        background-image:
            linear-gradient(rgba(0, 0, 0, 0) 30%, rgb(30, 48, 32) 70%), 
            url('../assets/bg-transparent-3.png')
        ;
        h1{
            font-family: 'Domine', serif;
            font-weight: normal;
            font-size: 50px;
        }
        li{
            width: calc(100% / 3);
            padding: 0 80px;
            img{
                width: 100px;
                border-radius: 60px;
            }
            p, span{
                font-size: 20px;
            }
            p{
                line-height: 30px;
            }
            span{
                color: $naturalGrey;
            }
        }
    }

</style>