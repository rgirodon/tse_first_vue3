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
      return this.reverseString(this.message);
    }    
  },

  methods : {
    reverseString(str) {
      return str.split("").reverse().join("");
    }
  }
}
</script>

<template>
  <div>
    <button @click="count++">Count is: {{ count }}</button>
    <p>{{ message }}</p>
    <p class="reversed">{{ reversedMessage }}</p>
  </div>
</template>

<style scoped>
p.reversed {
  font-style: italic;
}
</style>
