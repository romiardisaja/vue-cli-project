<template>
    <h2>Welcome {{ nama }}</h2>
    <!-- <button v-on:click="changeName">Change Name</button> -->
    <button @click="changeName">Change Name</button>
</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      nama: 'Romi'
    }
  },
  methods: {
    changeName(){
      this.nama = 'Rassya'
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
