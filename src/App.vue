<template>
  <div id="app">
    <location></location>
    <router-view/>
  </div>
</template>

<script>
import location from 'common/svg/location'

export default {
  name: 'App',
  components: {
    location
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
#app
  position: fixed
  width: 100vw
  height: 100vh
</style>
