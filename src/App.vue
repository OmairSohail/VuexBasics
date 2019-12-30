<template>
  <div id="app">
    <productlistone v-bind:products="products"></productlistone>
    <productlisttwo v-bind:products="products"></productlisttwo>  
  </div>
</template>

<script>
import productlistone from './components/ProductListOne'
import productlisttwo from './components/ProductListTwo'
export default {
  name: 'app',
  components: {
   productlistone,
   productlisttwo
  },
  data(){
    return{
      products:[
        {id:1,name:'Banana',price:20},
        {id:2,name:'Apple',price:30},
        {id:3,name:'Pineapple',price:40},
        {id:4,name:'GreyFruit',price:50},
        {id:5,name:'Chocolate',price:60},
        {id:6,name:'Basin',price:70},
        {id:7,name:'Chips',price:80}
        
      ]
    }
  }
}
</script>

<style>
#app {
 font-family: 'Teko', sans-serif;
 font-size:1.5rem;
}
</style>
