<template>
    <Header @headerChangeJudul="changeJudul" :judul="isiJudul" />
</template>

<script>
import Header from '@/components/Header.vue'

export default {
  name: 'App',  
  components:{
    Header
  },
  data(){
    return {
      isiJudul: "Ini adalah judul dari data"
    }
  },
  methods: {
    changeJudul(judulBaru){
      this.isiJudul = judulBaru;
    }
  },
}
</script>

<style>

</style>
