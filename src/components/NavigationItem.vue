<script setup lang="ts">
import { RouterLink } from 'vue-router'
import IconDonutChart from './icons/IconDonutChart.vue'
import IconCashRegister from './icons/IconCashRegister.vue'
import IconCoin from './icons/IconCoin.vue'
import IconCoins from './icons/IconCoins.vue'
import IconColumns from './icons/IconColumns.vue'
import IconNotebook from './icons/IconNotebook.vue'
import IconBuilding from './icons/IconBuilding.vue'
import IconDeviceDesktop from './icons/IconDeviceDesktop.vue'
import IconListCheck from './icons/IconListCheck.vue'
import IconUser from './icons/IconUser.vue'
import IconSettings from './icons/IconSettings.vue'
import IconLogin from './icons/IconLogin.vue'
import IconBrand from './icons/IconBrand.vue'
import ToggleTheme from './ToggleTheme.vue'
</script>
<template>
  <nav>
    <div>
      <IconBrand />
    </div>
    <header>
      <div>
        <RouterLink to="/"><IconDonutChart /></RouterLink>
      </div>
      <div class="selected">
        <RouterLink to="/tip-payments"><IconCashRegister /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconColumns /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconCoin /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconNotebook /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconBuilding /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconDeviceDesktop /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconCoins /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconListCheck /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconUser /></RouterLink>
      </div>
    </header>
    <footer>
      <ToggleTheme />
      <div>
        <RouterLink to="/tip-payments"><IconSettings /></RouterLink>
      </div>
      <div>
        <RouterLink to="/tip-payments"><IconLogin /></RouterLink>
      </div>
    </footer>
  </nav>
</template>

<style scoped>
div {
  padding: 0.2rem;
  border-radius: 12px;
  display: flex;
  justify-content: center;
}
div.selected {
  padding-left: 1rem;
  padding-right: 1rem;
  background-color: #ed6959;
  border-radius: 12px;
}
.icon-tabler-cash-register {
  color: #fff;
  border-radius: 5px;
}
nav {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100vh;
  padding: 1rem;
}
header,
footer {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
svg {
  color: #c1c1c1;
}
</style>
