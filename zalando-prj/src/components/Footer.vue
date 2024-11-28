<script setup>
const colorFooter = 'red'
</script>

<template>
  <footer>Made by <a href="www.lereacteur.io"> Le Reacteur</a></footer>
</template>

<style scoped>
footer {
  display: flex;
  justify-content: center;
  align-items: center;
  height: var(--footer-height);
  border: solid;
}

a {
  color: var(--main-orange);
  font-weight: bold;
}
</style>
