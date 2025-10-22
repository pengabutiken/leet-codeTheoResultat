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
  width:40%;
  font-family: "Google Sans Code", monospace;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;  
  
}
code{
      font-family: "Google Sans Code", monospace;
  
  font-weight: 300;
  font-style: normal;  
  
}
</style>
