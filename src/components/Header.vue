<template>
<header class="Header">
    <h1>Theos Leetcode Lösningar</h1>

</header>

</template>
<script setup>

</script>
<style scoped>
.Header{
    
    background-color: #ce8507;
  color: rgb(255, 255, 255);
  padding-top: 10px;
  padding-bottom: 5px;
  font-size: 0.7rem;
  font-weight: 100;
  width: 100%;
   font-family: "Press Start 2P", system-ui;

}
h1{
  font-size: 3em;
  background: linear-gradient(90deg, red, orange, yellow, green, blue, indigo, violet);
  background-size: 400%;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  transition: background-position 1s;
}
h1:hover {
  animation: rainbow 2s linear infinite;
}
@keyframes rainbow {
  0% {
    background-position: 0%;
  }
  100% {
    background-position: 100%;
  }
}



</style>