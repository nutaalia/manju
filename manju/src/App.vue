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
header {
  display: flex;
  width: 100vw;
  height: 100vh; 
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.jul,
.manu {
  flex: 0 0 50%; 
  height: 100%;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1rem;
}

.jul {
  border-right: 1px solid #ccc;
}


html, body, #app {
  height: 100%;
  margin: 0;
}
</style>
