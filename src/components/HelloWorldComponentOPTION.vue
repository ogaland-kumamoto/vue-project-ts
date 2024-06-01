<!-- HelloWorldComponent.vue -->
<template>
  <h1>{{ msg }}</h1>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
data() {
  return {
    // 型宣言できない
    msg: 'Hello World!'
  }
},
methods: {
  increment(num: number) {
    return num + 1;
  }
},
mounted() {

  console.log(this.increment("999"));
}
})
</script>

<style scoped>

</style>