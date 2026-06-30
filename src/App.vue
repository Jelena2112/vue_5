<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <ProductsPage  />

</template>

<script>
import ProductsPage from '@/components/ProductsPage.vue'


export default {
  name: 'App',
  components: {ProductsPage},
  provide() {
    return {
      ProvidedProductList: this.ProductsList
    }
  },
  data: () => ({
    ProductsList: [
      {
        name: "Laptop",
        price: 1200,
        length: 35,
        discount: null
      },
      {
        name: "Smartphone",
        price: 800,
        length: 15,
        discount: "50%"
      },
      {
        name: "Headphones",
        price: 150,
        length: 20,
        discount: null
      },
      {
        name: "Keyboard",
        price: 90,
        length: 45,
        discount: "50%"
      },
      {
        name: "Mouse",
        price: 50,
        length: 12,
        discount: null
      },
    ],
  })

}
</script>


