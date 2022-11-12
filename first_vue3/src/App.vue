<script>
export default {
  data() {
    return {
      title: "Vue Router"
    }
  }
}
</script>

<template>
  <h1>{{ title }}</h1>
  <nav>
    <router-link to="/">Go to Home</router-link>
    <router-link to="/about">Go to About</router-link>
  </nav>
  <router-view></router-view>
</template>

<style scoped>
a + a {
  margin-left: 10px;
}
</style>
