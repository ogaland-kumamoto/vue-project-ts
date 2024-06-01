<!-- HelloWorldComponent.vue -->
<script setup lang="ts">

// 静的型付けの確認
let msg: number
msg = 'Hello World!'


// 値の型を指定しているが、実際には文字列を返している
function increment(num: number) {
//                 ^^^^^^^^型注釈
  return num + 1;
}

console.log(increment("999"));

</script>

<template>
    <h1>{{ msg }}</h1>
</template>

<style scoped>

</style>