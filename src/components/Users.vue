<template>
 <p>{{ msg }}</p>
  <Info :currentDate="currentDate"></Info>/
<!--  <p>{{ currentDate }}</p>-->

  <Info></Info>
</template>

<script>
import Info from "@/components/Info.vue";

export default {
  name: 'Users',
  components: {Info},
  props: {
    msg: String,
    currentDate: String
  }
}
</script>


