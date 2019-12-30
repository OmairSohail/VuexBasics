<template>
    <div id="productlistone">
      <h1>Product List One</h1>
      <ul>
          <li v-for="product in products" :key="product.id">
              <span class="name">{{product.name}}</span>
              <span class="price">Rps-{{product.price}}</span>
          </li>
      </ul>
    </div>
</template>

<script>
export default {
      props:['products'] ,
      data(){
          return{

          }
      }   
}
</script>

<style scoped>
.price{
    margin-left:3rem;

}
</style>