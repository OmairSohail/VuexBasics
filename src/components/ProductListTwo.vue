<template>
    <div id="productlisttwo">
      <h1>Product List Two</h1>
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
        props:['products']  
}
</script>

<style scoped>
.price{
    margin-left:3rem;

}
</style>