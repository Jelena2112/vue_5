<template>

    <div v-for="product in ProvidedProductList" :key="product.id">
      <ProductInfo :product="product" />
    </div>

</template>

<script>
export default {
  name: 'ProductDetails',
  inject: ['ProvidedProductList'],

}
</script>