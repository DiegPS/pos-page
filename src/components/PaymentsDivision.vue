<script setup lang="ts">
import AmountItem from '@/components/AmountItem.vue'
import IconPencil from './icons/IconPencil.vue'
import IconWallet from './icons/IconWallet.vue'
defineProps<{
  amount: string[]
}>()
</script>
<template>
  <section>
    <header>
      <article>
        <p>Total de Propinas</p>
        <div>
          <AmountItem :amount="amount.join('')" />
          <IconPencil />
        </div>
      </article>
      <h3>¿Entre cúantos quieres dividir las Propinas?</h3>
      <input />
    </header>
    <footer>
      <IconWallet />
      <h3>Elige el Método de Pago</h3>
    </footer>
  </section>
</template>
<style scoped>
section {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
.icon {
  width: 2rem;
  height: 2rem;
}
footer {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}
div {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}
svg {
  color: #3d3d3d;
}
article {
  display: flex;
  flex-direction: column;
  align-items: center;
}
h3 {
  color: #3d3d3d;
  font-weight: 700;
}
p {
  color: #ed6959;
  font-weight: 700;
}
</style>
