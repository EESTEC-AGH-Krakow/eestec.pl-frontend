<template>
  <div id="app">
        <b-container fluid id="app" class="p-0">
        <!--        <headroom>-->
        <header class="sticky-top">
            <MyHeader/>
        </header>
        <!--        </headroom>-->
        <main>
            <router-view></router-view>
        </main>
        <footer>
            <MyFooter/>
        </footer>
    </b-container>
    <img alt="EESTEC logo" src="./assets/eestec-logo.png">
    <h2>EESTEC</h2>
    <AboutUs />
  </div>
</template>

<script>
import AboutUs from './components/AboutUs.vue'
import MyHeader from './components/MyHeader.vue'
  import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    AboutUs,
    MyHeader,
    MyFooter
  }
}
</script>

<style scoped lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background: #acadae;
}


</style>
