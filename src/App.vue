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
      <SectionTen />
      <SectionEleven :mainArray="infoIcons"/>
      <SectionTwelve :mainArray="articles3"/>
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
import SectionTen from '@/components/SectionTen.vue'
import SectionEleven from '@/components/SectionEleven.vue'
import SectionTwelve from '@/components/SectionTwelve.vue'

import {navLink} from '@/Data/allArrays'
import {articles1} from '@/Data/allArrays'
import {articles2} from '@/Data/allArrays'
import {articles3} from '@/Data/allArrays'
import {blogs} from '@/Data/allArrays'
import {foods} from '@/Data/allArrays'
import {users} from '@/Data/allArrays'
import {infoIcons} from '@/Data/allArrays'

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
    SectionTen,
    SectionEleven,
    SectionTwelve,
  },
  data() {
    return{
      navLink,
      articles1,
      articles2,
      articles3,
      blogs,
      foods,
      users,
      infoIcons,
    }
  } 
}
</script>

<style lang="scss">
@import '@/Style/globals.scss'

</style>
