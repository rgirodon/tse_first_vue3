<script>
export default {
  data() {
    return {
      random: Math.floor(Math.random() * 100)
    }
  },
  methods: {
    isLifeAwesome() {
      return (this.random % 2 == 0);
    },
    refreshRandom() {
      this.random = Math.floor(Math.random() * 100);
    }
  }
}
</script>

<template>
  <div>  
    <h1 v-if="isLifeAwesome()">Life is awesome !</h1>
    <h1 v-else>Life is so sad !</h1>
    <button @click="refreshRandom">Refresh</button>
  </div>
</template>

<style scoped>
</style>
