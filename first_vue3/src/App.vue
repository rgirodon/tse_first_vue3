<script>
export default {
  data() {
    return {
      count: 0,
      shoppingList: [{ key:1, article: 'Lessive' }, { key:2, article: 'Lait' }]
    }
  }
}
</script>

<template>
  <div>
    <button @click="count++">Count is: {{ count }}</button>
    <ul>
      <li v-for="item in shoppingList" :key="item.id">{{ item.article }}</li>
    </ul>
  </div>
</template>

<style scoped>
</style>
