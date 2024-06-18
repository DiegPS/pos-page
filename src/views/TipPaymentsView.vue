<script setup lang="ts">
import { ref } from 'vue'
import TouchNumbers from '../components/TouchNumbers.vue'
import AmountItem from '@/components/AmountItem.vue'

let amount = ref<string[]>([])

const updateAmount = (newAmount: string[]) => {
  amount.value = newAmount
}
</script>

<template>
  <main>
    <AmountItem :amount="amount.join('')" />
    <TouchNumbers @update="updateAmount" />
    <div>Seleccionado: {{ amount.join(', ') }}</div>
  </main>
</template>
