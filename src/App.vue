<template>
  <div id="app">
    <Header :links="navLink"/>

    <main>
      <SectionOne />
      <SectionTwo />
      <SectionThree :mainArray="articles1"/>
      <SectionFour :arrayElements="foods"/>
      <SectionFive />
      <SectionSix :mainArray="articles2"/>
      <SectionSeven :mainArray="users"/>
      <SectionEight />
      <SectionNine :mainArray="blogs"/>
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import SectionOne from '@/components/SectionOne.vue'
import SectionTwo from '@/components/SectionTwo.vue'
import SectionThree from '@/components/SectionThree.vue'
import SectionFour from '@/components/SectionFour.vue'
import SectionFive from '@/components/SectionFive.vue'
import SectionSix from '@/components/SectionSix.vue'
import SectionSeven from '@/components/SectionSeven.vue'
import SectionEight from '@/components/SectionEight.vue'
import SectionNine from '@/components/SectionNine.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    SectionSeven,
    SectionEight,
    SectionNine,
  },
  data() {
    return{
      navLink: ['Home', 'Shop', 'About', 'Blog','Contact', 'Shop by brand'],

      articles1: [
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
      ],

      articles2: [
        {
          src: '/product-21.jpg',
          title: 'Transport cage',
          price: '$25.00',
        },
        {
          src: '/product-20.jpg',
          title: 'Dog leash',
          price: '$25.00',
        },
        {
          src: '/product-16.jpg',
          title: 'Animal transport cage',
          price: '$25.00',
          originalPrice: '$35.00',
        },
        {
          src: '/product-11.jpg',
          title: 'Colorful cat leash',
          price: '$12.00',
        }
      ],

      blogs: [
        {
          src: '/blog-1.jpg',
          title: "How to 'loose leash walk' your dog",
          date: 'April 21st, 2020',
        },
        {
          src: '/blog-2.jpg',
          title: 'Stop cats from scratching furniture',
          date: 'April 19st, 2020',
        },
        {
          src: '/blog-3.jpg',
          title: 'Where to buy the best pet food',
          date: 'April 18st, 2020',
        },
        {
          src: '/blog-4.jpg',
          title: 'Proper care for your pet toys',
          date: 'April 17st, 2020',
        }
      ],

      foods: [
        {
          srcFood: '/food-transparent-18.png',
          title: 'Kibble',
          description: 'Dry dog food',
          btnText: 'Shop dry food'
        },
        {
          srcFood: '/food-transparent-17.png',
          title: 'Moist',
          description: 'Canned do food',
          btnText: 'Shop moist food'
        },
        {
          srcFood: '/food-transparent-16.png',
          title: 'Frozen',
          description: 'Freeze-Dried do food',
          btnText: 'Shop frozen food'
        }
      ],

      users: [
        {
          userSrc: '/avatar-3.jpg',
          info: 'Lisa Smith consectetur adipisicing elit. Labore maxime modi porro totam reiciendis dolore aliquam itaque quos inventore illum?',
          name: 'Lisa Smith, ThemeFusion'
        },
        {
          userSrc: '/avatar-1.jpg',
          info: 'Melissa Green consectetur adipisicing elit. Labore maxime modi porro totam reiciendis dolore aliquam itaque quos inventore illum?',
          name: 'Melissa Green, ThemeFusion'
        },
        {
          userSrc: '/avatar-4.jpg',
          info: 'Sam Lewis consectetur adipisicing elit. Labore maxime modi porro totam reiciendis dolore aliquam itaque quos inventore illum?',
          name: 'Sam Lewis, ThemeFusion'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import '@/Style/globals.scss'

</style>
