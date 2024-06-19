<script setup lang="ts"></script>

<template>
  <section>
    <aside>
      <header>
        <p>Total pagado</p>
        <p>amount</p>
      </header>
      <footer>
        <p>Restante por pagar</p>
        <p>amount</p>
      </footer>
    </aside>
    <button>Pagar Propinas</button>
  </section>
</template>
<style scoped>
p {
  font-size: 1.8rem;
  font-weight: 700;
}
aside {
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
  width: 40rem;
}
header {
  color: #ed6959;
  display: flex;
  justify-content: space-between;
}
footer {
  display: flex;
  justify-content: space-between;
  color: #3d3d3d;
}
button {
  border: 3px solid #c1c1c1;
  border-radius: 30px;
  padding: 0.8rem 3rem;
  font-size: 2rem;
  font-weight: 700;
  color: #c1c1c1;
}
section {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  padding: 0rem 2rem;
}
</style>
