<script setup>
import Julia from './components/Julia.vue'
import Manuel from './components/Manuel.vue'
</script>

<template>
  <header>
    <div class="jul">
      <Julia />
    </div>

    <div class="manu">
      <Manuel />
    </div>
  </header>
</template>

<style scoped>
:global(html), 
:global(body), 
:global(#app) {
  margin: 0 !important;
  padding: 0 !important;
  width: 100% !important;
  max-width: none !important;
  height: 100%;
  overflow-x: hidden;
}

header {
  display: flex;
  width: 100vw;
  height: 100vh;
  margin: 0;
  padding: 0;
}

.jul,
.manu {
  flex: 1;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-sizing: border-box;
}

.jul {
  border-right: 1px solid #ccc;
}
</style>
