<script setup>
  import {ref} from "vue";
  const count = ref(0)
  const addCount = () => {
    count.value += 1;
  }
  const substractCount = () => {
    count.value -= 1;
  }
</script>


<template>
  <main>
    <div>
      <h4>The current count is...</h4>
      <h1>{{ count }}</h1>
      <button @click="substractCount">-</button>
      <button @click="addCount">+</button>
    </div>
  </main>
</template>

<style scoped>
  main{
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
  }
</style>
