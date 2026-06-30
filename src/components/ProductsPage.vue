<template>
  <DiscountedProducts />
  <ProductDetails />
</template>

<script>
import ProductDetails from '@/components/ProductDetails.vue'
import DiscountedProducts from '@/components/DiscountedProducts.vue'
 export default {
   name: 'ProductsPage',
   components: {ProductDetails, DiscountedProducts},


 }
</script>