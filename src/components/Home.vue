<template>
  <div class="jjjj">
    <public-header></public-header>
      <div>{{msg}}</div>
  </div>
</template>

<script>
import PublicHeader from './public/publicHeader'
export default {
  name: 'Home',
  components: {PublicHeader},
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
