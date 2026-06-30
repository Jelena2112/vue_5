<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <ProductsPage  />

</template>

<script>
import ProductsPage from '@/components/ProductsPage.vue'


export default {
  name: 'App',
  components: {ProductsPage},
  data: () => ({
    ProductsList: [
      {
        name: "HTML Course",
        price: 150,
        length: "2 months",
      },
      {
        name: "CSS Course",
        price: 180,
        length: "3 months",
      },
      {
        name: "JavaScript Course",
        price: 250,
        length: "5 months",
      },
      {
        name: "React Course",
        price: 350,
        length: "4 months",
      },
      {
        name: "Vue.js Course",
        price: 300,
        length: "2 months",
      },
    ],
  })

}
</script>


