<template>
  <input type="text" v-model="cari" placeholder="Cari Product">
  <ul>
    <li v-for="item in cariData" :key="item.id">
      {{ item.title }} - {{ item.price }}
    </li>
  </ul>
  
</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      cari: '',
      products: []
    }
  },
  created(){
    console.log('created');
    this.products = [
      {id: 1, title: "Product 1", price: 1000},
      {id: 2, title: "Product 2", price: 2000},
      {id: 3, title: "Product 3", price: 3000},
      {id: 4, title: "Product 4", price: 4000},
      {id: 5, title: "Product 5", price: 5000},
    ]
  },
  computed: {
    cariData(){
      return this.products.filter(item => {
        return item.title.match(this.cari);
      });
    }
  }
}
</script>

<style>

</style>
