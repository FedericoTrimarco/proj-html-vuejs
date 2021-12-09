<template>
  <div id="app">
    <Header :links="navLink"/>

    <main>
      <SectionOne />
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import SectionOne from '@/components/SectionOne.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionOne,
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
