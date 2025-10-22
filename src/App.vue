<template>
  <div id="app">
    <Header></Header>
    <div class="content">
      <section class="row">
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
    ></Solution> </section>
    <section class="row">
    <Problem title="Palidrome Number" description="Given an integer x, return true if x is a palindrome, and false otherwise."></Problem>
    </section>
    </div>
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
  
  background-color: gray;

  
}
.content{
  display: flex;
  flex-direction: column;
  gap: 40px; 
  padding: 20px;
  
}
.row{
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 20px;
}
</style>
