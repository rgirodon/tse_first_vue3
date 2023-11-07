<script>
export default {
  data() {
    return {
      shoppingList: [
        { key:1, article: 'Lessive' }, 
        { key:2, article: 'Lait' },
        { key:3, article: 'Chocolat' },
        ]
    }
  }
}
</script>

<template>
  <div>
    <ul>
      <li v-for="item in shoppingList" :key="item.key">{{ item.article }}</li>
    </ul>
  </div>
</template>

<style scoped>
</style>
