<template>
  <p>Trenutni datum je: {{ currentDate }}</p>
  <div class="info">Info component</div>
</template>

<script>
  export default {
    name: 'Info',
    props:{
      currentDate: String
    }
  }
</script>