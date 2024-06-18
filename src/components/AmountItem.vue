<script setup lang="ts">
defineProps<{
  amount: string
}>()
</script>
<template>
  <button>
    <aside><p>$</p></aside>
    <h2>{{ Number(amount).toLocaleString('en-US', { minimumFractionDigits: 2 }) }}</h2>
  </button>
</template>

<style scoped>
button {
  background-color: #fbddda;
  display: flex;
  border: 0px;
  border-radius: 4px;
}
p {
  font-size: 2rem;
  font-weight: 700;
  color: #ed6959;
}
aside {
  display: flex;
  justify-content: center;
  align-items: center;
}

h2 {
  font-size: 2rem;
  font-weight: 700;
  color: #ed6959;
}
</style>
