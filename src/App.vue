<template>
  <div id="app">
    <Header></Header>
    <Problem
      title="Two Sum"
      description="Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target."
    ></Problem>
  </div>
</template>
<script setup>
import Header from "./components/Header.vue";
import Problem from "./components/Problem.vue";
</script>
<style>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: black;
}
</style>
