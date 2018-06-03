<template>
  <div class="home">
    <Banner />
    <Tabs/>
    <comoFunciona />
    <packs/>
    <Newsletter />
    <Footer/>
    <PostFooter/>
  </div>
</template>

<script>
import Banner from '../components/Banner'
import Tabs from '../components/Tabs'
import comoFunciona from '../components/comoFunciona'
import packs from '../components/packs'
import Newsletter from '../components/newsletter'
import Footer from '../components/Footer'
import PostFooter from '../components/PostFooter'
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
      packs,
      Newsletter,
      Footer,
      PostFooter
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
