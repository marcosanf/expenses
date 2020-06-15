<template>
  <div id="app">
    <h3>oi</h3>
    <div id="nav">
    <base-spinner/>
    <router-view/>
  </div>
  </div>

</template>

<script>
import BaseSpinner from './components/global/BaseSpinner'
export default {
  name: 'App',
  components: {
    BaseSpinner
  },
  mounted () {
    console.log(this.$firebase)
  }
}

</script>

<style lang="scss">
#app {
  min-height: 100vh;
  color: var(--light);
  background-color: var(--darker);
}

</style>
