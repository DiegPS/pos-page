<script setup lang="ts">
import { RouterLink } from 'vue-router'
import DocumentationIcon from './icons/IconDocumentation.vue'
</script>
<template>
  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
    <RouterLink to="/tip-payments">Tip Payments</RouterLink>
    <RouterLink to="/settings">Settings</RouterLink>
    <RouterLink to="/account">Account</RouterLink>
    <RouterLink to="/login">Login</RouterLink>
  </nav>
  <DocumentationIcon />
</template>
