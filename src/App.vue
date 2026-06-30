<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <Users msg="Welcome to Your Propppppp" :currentDate="currentDate"/>
</template>

<script>
import Users from './components/Users.vue'

export default {
  name: 'App',
  data:() => ({
    currentDate:'01/01/2025'
  }),
  components: {
    Users
  }
}
</script>


