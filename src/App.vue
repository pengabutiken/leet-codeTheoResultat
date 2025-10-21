<template>
  <div id="app">
    <Header></Header>
    <Problem
      title="Two Sum"
      description="Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target."
    ></Problem>
    <Solution
      solution="var twoSum = function(nums, target) {
for(let i =0; i<nums.length;i++){
    for(let j=i+1;j<nums.length;j++){
        if(nums[i]+nums[j]==target){
            return [i,j]
        }
    }
}
return [];
    }
"
    ></Solution>
  </div>
</template>
<script setup>
import Header from "./components/Header.vue";
import Problem from "./components/Problem.vue";
import Solution from "./components/Solution.vue";

</script>
<style>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: black;
}
</style>
