<template>
  <div class="home">
    <Banner />
    <Tabs/>
    <comoFunciona />
    <packs/>
  </div>
</template>

<script>
import Banner from '../components/Banner'
import Tabs from '../components/Tabs'
import comoFunciona from '../components/comoFunciona'
import packs from '../components/packs'
export default {
  name: 'home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
      Banner,
      Tabs,
      comoFunciona,
      packs
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
