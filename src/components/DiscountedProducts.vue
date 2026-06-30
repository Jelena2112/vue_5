<template>\
  <h3>Discounted Products</h3>
  <div v-for="product in ProvidedProductList" :key="product.id">
    <ProductInfo :product="product" />
  </div>
</template>

<script>



import ProductInfo from "@/components/ProductInfo.vue";

export default {
  name: 'DiscountedProducts',
  components: {ProductInfo},
  inject: ['ProvidedProductList'],
  computed: {
    discountedProducts() {
      return this.ProvidedProductList.filter(product => product.discount !== null)
    }
  }
}
</script>