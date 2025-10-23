<template> 

<div>

    <h6> <span class="material-symbols-outlined">
timer
</span> {{ time }}</h6>
<p>{{ comments }}</p>
</div>
</template>

<script setup>
defineProps({
    comments:String,
    time:String
})
</script>


<style scoped>
div{
    width: 100%;
    background-color: white;
    padding: 20px;
    font-family: "Google Sans Code",serif ;
    font-style: italic;
    font-weight: 100;
    font-size: 12px;

}
span{
    font-size:20px;
    line-height: 2;
    font-weight: bold;
}
h6{
    font-style: none;
    font-weight: bold;
    font-size: 15px;
}
</style>