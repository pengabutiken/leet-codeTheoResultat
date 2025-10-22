<template>
  <div class="solution-card">
    <h2>Solution</h2>
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
  background-color: #ffffff;
  width:60%;
  font-family: "Google Sans Code", monospace;
  font-optical-sizing: auto;
  font-weight: 300;
  font-style: normal;  
  padding: 10px 20px ;
}
code{
      font-family: "Google Sans Code", monospace;
  
  font-weight: 300;
  font-style: normal;  
  font-size: 12px;
  
}
</style>
