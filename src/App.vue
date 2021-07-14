<template>
  <div id="app">
    <Header></Header>
    <Body align="center"></Body>
    <Footer></Footer>
  </div>
</template>

<script>

import Header from './components/header/header.vue'
import Footer from './components/footer/footer.vue'
import Body from './components/body/body.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Body
  }
}
</script>


