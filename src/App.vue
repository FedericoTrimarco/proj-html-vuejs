<template>
  <div id="app">
    <Header :links="navLink"/>

    <main>
      <SectionOne />
      <SectionTwo 
        title="Browse by category"
        description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores laudantium, reprehenderit nam ad ipsam iste perferendis aut dolorum adipisci delectus veniam nulla."
      />
      <SectionThree :mainArray="articles1"/>
      <SectionFour :arrayElements="foods"/>
      <SectionFive />
      <SectionSix :mainArray="articles2"/>
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
      ]
    }
  }
}
</script>

<style lang="scss">
@import '@/Style/globals.scss'

</style>
