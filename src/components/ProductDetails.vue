<template>
  <ul>
    <li v-for="product in ProvidedProductList" :key="product.id">
      {{ product.name }} - ${{ product.price }} - {{ product.length }}
    </li>

  </ul>
</template>

<script>
export default {
  name: 'ProductDetails',
  inject: ['ProvidedProductList'],

}
</script>