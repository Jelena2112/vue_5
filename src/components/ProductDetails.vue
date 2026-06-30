<template>
  <div>Product details</div>
</template>

<script>
export default {
  name: 'ProductDetails',
  inject: ['ProvidedProductList'],
  mounted() {
    console.log(this.ProvidedProductList);
  }
}
</script>