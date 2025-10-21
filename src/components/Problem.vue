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
  padding: 15px;
  border-radius: 8px;
}
</style>