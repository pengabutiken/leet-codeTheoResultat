<template>
    <div class="problem-card">

        <h2>{{ title }}</h2>
        <p> {{ description }}</p>
    </div>

</template>

<script setup>
defineProps({
    title:String,
    description:String,

})

</script>
<style scoped>
.problem-card {
  background-color: #f0f0f0;
    font-family: "Vend Sans", sans-serif;
  
  width: 50%;
}
</style>