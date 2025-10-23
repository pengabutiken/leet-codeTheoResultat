<template> 
<p>{{ comments }}</p>

</template>

<script setup>
defineProps({
    comments:String
})
</script>


<style scoped>
p{
    width: 100%;
    background-color: white;
    padding: 20px;
    font-family: "Google Sans Code",serif ;
    font-style: italic;
    font-weight: 100;
    font-size: 12px;
}
</style>