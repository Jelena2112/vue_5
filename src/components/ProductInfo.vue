<template>
  <div>{{ product.name }}</div>
  <div>{{ product.price }}</div>
  <div>{{ product.length }}</div>
</template>


<script>
export default {
  name: 'ProductInfo',
  props: {
    product:Object
  }
}
</script>
