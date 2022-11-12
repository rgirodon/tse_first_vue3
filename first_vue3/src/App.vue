<script>
import CounterComponent from './components/CounterComponent.vue';

export default {
  data() {
    return {
      message: "Hello TSE !"
    }
  },
  components: {
    CounterComponent
  }
}
</script>

<template>
  <p>The message : {{ message }}</p>
  <counter-component :initial="0" :increment="1" />
  <counter-component :initial="0" :increment="2" />
  <counter-component :initial="100" :increment="-1" />
</template>

<style scoped>
p {
  font-style: italic;
}
</style>
