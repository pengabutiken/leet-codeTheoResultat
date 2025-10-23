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
        ></Solution>
      </section>
      <Comment comments="// tänkte som i en bubbel sort och efter det blev det ganska simpelt."> </Comment>

      <section class="row">
        <Problem
          title="Palidrome Number"
          description="Given an integer x, return true if x is a palindrome, and false otherwise."
        ></Problem>
        <Solution
          solution="var isPalindrome = function(x) {
    let ord=x.toString();
    let bak=ord.split('').reverse().join('');
    if(ord===bak){
        return true;
    }else {
        return false;
    }"
        ></Solution>
      </section>
      <section class="row">
        <Problem title="Roman to Integer" description="Roman numerals are
        represented by seven different symbols: I, V, X, L, C, D and M. Symbol
        Value I 1 V 5 X 10 L 50 C 100 D 500 M 1000 For example, 2 is written as
        II in Roman numeral, just two ones added together. 12 is written as XII,
        which is simply X + II. The number 27 is written as XXVII, which is XX +
        V + II. Roman numerals are usually written largest to smallest from left
        to right. However, the numeral for four is not IIII. Instead, the number
        four is written as IV. Because the one is before the five we subtract it
        making four. The same principle applies to the number nine, which is
        written as IX. There are six instances where subtraction is used: I can
        be placed before V (5) and X (10) to make 4 and 9. X can be placed
        before L (50) and C (100) to make 40 and 90. C can be placed before D
        (500) and M (1000) to make 400 and 900. Given a roman numeral, convert
        it to an integer." ></Problem>
        <Solution solution="var romanToInt = function(s) {
    const symboler={
    I:1,
    V:5,
    X :10,
    L:50,
    C:100,
    D:500,
    M:1000
    };
    let total=0;
    for(let i=0;i<s.length;i++){
        let nuvar=s[i];
        let nesta=s[i+1];
        if(symboler[nuvar]<symboler[nesta]){
            total-=symboler[nuvar];
        }else{
            total+=symboler[nuvar];
        }
    }
    return total;

};"></Solution>
      </section>
    </div>
  </div>
</template>
<script setup>
import Header from "./components/Header.vue";
import Problem from "./components/Problem.vue";
import Solution from "./components/Solution.vue";
import Comment from "./components/Comment.vue";
</script>
<style>
body {
  margin: 0;
  padding: 0;

  background-color: gray;
}
.content {
  display: flex;
  flex-direction: column;
  gap: 40px;
  padding: 20px;
}
.row {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 20px;
}
</style>
