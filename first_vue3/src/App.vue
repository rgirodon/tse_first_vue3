<script>
export default {
  
  data() {
    return {
      count: 0,
      message: "Hello"
    }
  },

  computed : {
    reversedMessage() {
      return this.message.split("").reverse().join("");
    }    
  },

  methods : {
    increment() {
      this.count++;
    }
  }
}
</script>

<template>
  <div>
    <button @click="increment">Count is: {{ count }}</button>
    <p>{{ message }}</p>
    <p class="reversed">{{ reversedMessage }}</p>
  </div>
</template>

<style scoped>
p.reversed {
  font-style: italic;
}
</style>
