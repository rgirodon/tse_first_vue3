<script>
export default {
  data() {
    return {
      count: 0,
      name: "",
      displayedName: "" 
    }
  },
  methods: {
    copyNameToDisplayedName() {
      this.displayedName = this.name;
    }
  }
}
</script>

<template>
  <div>
    <button @click="count++">Count is: {{ count }}</button>

    <div>
      <input v-model="name">
      <button @click="copyNameToDisplayedName">Reveal</button>
      <p>You are : {{ displayedName }}</p>
    </div>
  </div>
</template>

<style scoped>
</style>
