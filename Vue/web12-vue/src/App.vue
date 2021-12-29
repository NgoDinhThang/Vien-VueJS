<template>
  <div id="app">
    <LayOutLeft/>
    <LayOutRight/>
  </div>
</template>

<script>
import LayOutLeft from './components/layout/TheLayOutLeft.vue'
import LayOutRight from './components/layout/TheLayOutRight.vue'

export default {
  name: 'App',
  components: {
    LayOutLeft,LayOutRight
  }
}
</script>

<style>
#app{
  display: flex;
}
</style>
