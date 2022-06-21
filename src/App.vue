<template>
  <div>
      <TheHeader></TheHeader>
      <BlackLine></BlackLine>
      <BlueLine></BlueLine>
      <BgLink></BgLink>
      <TheFooter></TheFooter>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import BlackLine from './components/BlackLine.vue'
import BlueLine from './components/BlueLine.vue'
import BgLink from './components/BgLink.vue'


export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    BlackLine,
    BlueLine,
    BgLink
  }
}
</script>

<style lang="scss">

@import "assets/main.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
