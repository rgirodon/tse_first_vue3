<script>
export default {
  data() {
    return {
      count: 0
    }
  },
  methods: {
    isLifeAwesome() {
      return (Math.floor(Math.random() * 100) % 2 == 0);
    }
  }
}
</script>

<template>
  <div>  
    <h1 v-if="isLifeAwesome()">Life is awesome !</h1>
    <h1 v-else>Life is so sad !</h1>
    <button @click="count++">Count is: {{ count }}</button>
  </div>
</template>

<style scoped>
</style>
