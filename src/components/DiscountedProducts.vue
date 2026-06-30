<template>\
  <h3>Discounted Products</h3>
  <ul>
    <li v-for="product in discountedProducts" :key="product.id" >
      {{ product.name }} - ${{ product.price }} - {{ product.length }}
    </li>
  </ul>
</template>

<script>



export default {
  name: 'DiscountedProducts',
  inject: ['ProvidedProductList'],
  computed: {
    discountedProducts() {
      return this.ProvidedProductList.filter(product => product.discount !== null)
    }
  }
}
</script>