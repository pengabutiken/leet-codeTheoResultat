<template>
  <div class="solution-card">
    <h2>Lösning</h2>
    <pre><code>{{ solution }}</code></pre>
  </div>
</template>

<script setup>
defineProps({
  solution: String
})
</script>

<style scoped>
.solution-card {
  background-color: #e8f5e9;
  padding: 15px;
  border-radius: 8px;
  white-space: pre-wrap; 
}
</style>
