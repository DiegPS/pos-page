<script setup lang="ts">
import IconWallet from './icons/IconWallet.vue'
import IconCash from './icons/IconCash.vue'
import IconCreditCard from './icons/IconCreditCard.vue'
import TotalTips from './TotalTips.vue'
defineProps<{
  amount: string[]
}>()
</script>
<template>
  <section>
    <TotalTips :amount="amount" />
    <header>
      <h3>¿Entre cúantos quieres dividir las Propinas?</h3>
      <input />
    </header>
    <footer>
      <IconWallet />
      <h3>Elige el Método de Pago</h3>
    </footer>
    <article>
      <span><IconCash />Efectivo</span>
      <span><IconCreditCard />Santander 2323</span>
      <span><IconCreditCard /> BBVA 3213</span>
    </article>
  </section>
</template>
<style scoped>
article {
  display: grid;
  gap: 1rem;
  grid-template-columns: 1fr 1fr;
}
span {
  display: flex;
  flex-direction: column;
  align-items: center;
  min-height: 3rem;
  justify-content: center;
  border-radius: 8px;
  box-shadow: 0 0 5px #3d3d3d;
  font-weight: 700;
  color: #3d3d3d;
  padding: 1rem;
}
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

svg {
  color: #3d3d3d;
}

h3 {
  color: #3d3d3d;
  font-weight: 700;
}
</style>
