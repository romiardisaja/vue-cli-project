<template>
    <!-- <a v-bind:href="url">GO TO GOOGLE</a> -->
    <a :href="url">GO TO GOOGLE</a>
</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      url: 'https://google.com'
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
