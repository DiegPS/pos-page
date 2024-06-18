<script setup lang="ts">
import NavigationItem from './components/NavigationItem.vue'
import { RouterView } from 'vue-router'
</script>

<template>
  <div class="wrapper">
    <NavigationItem />
  </div>
  <RouterView />
</template>
