<template>
  <div id="app">
    <Header :links="navLink"/>

    <main>
      <SectionOne />
      <SectionTwo />
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import SectionOne from '@/components/SectionOne.vue'
import SectionTwo from '@/components/SectionTwo.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionOne,
    SectionTwo,
  },
  data() {
    return{
      navLink: ['Home', 'Shop', 'About', 'Blog','Contact', 'Shop by brand']
    }
  }
}
</script>

<style lang="scss">
@import '@/Style/globals.scss'

</style>
