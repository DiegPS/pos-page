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

<style scoped>
*,
*::before,
*::after {
  box-sizing: border-box;
}

* {
  margin: 0;
}

body {
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}

img,
picture,
video,
canvas,
svg {
  display: block;
  max-width: 100%;
}

input,
button,
textarea,
select {
  font: inherit;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  overflow-wrap: break-word;
}

#root,
#__next {
  isolation: isolate;
}
</style>
