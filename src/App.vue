<template>
  <div id="app">
    <MainHeader />
    <ImageInput />
  </div>
</template>

<script>
import ImageInput from './components/ImageInput.vue'
import MainHeader from './components/MainHeader.vue'

export default {
  name: 'App',
  components: {
    ImageInput,
    MainHeader
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
