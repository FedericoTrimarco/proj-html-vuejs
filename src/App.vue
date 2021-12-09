<template>
  <div id="app">
    <Header :links="navLink"/>

    <main>
      <SectionOne />
      <SectionTwo />
      <SectionThree :mainArray="images"/>
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import SectionOne from '@/components/SectionOne.vue'
import SectionTwo from '@/components/SectionTwo.vue'
import SectionThree from '@/components/SectionThree.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionOne,
    SectionTwo,
    SectionThree,
  },
  data() {
    return{
      navLink: ['Home', 'Shop', 'About', 'Blog','Contact', 'Shop by brand'],
      images: [
                {
                    src: '/product-8.jpg',
                    title: 'Bed(1)',
                },
                {
                    src: '/product-3.jpg',
                    title: 'Food(6)',
                },
                {
                    src: '/product-2.jpg',
                    title: 'Toys(6)',
                },
                {
                    src: '/product-4.jpg',
                    title: 'Transport(6)',
                }
            ]
    }
  }
}
</script>

<style lang="scss">
@import '@/Style/globals.scss'

</style>
