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
  background-color: #ffffff;
       font-family: "Google Sans Code", monospace;
       font-weight: 300;
  padding: 30px;
  width: 50%;
}
</style>