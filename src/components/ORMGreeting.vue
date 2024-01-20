<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>One Repetition Max (1RM)</h3>
    <h4>(or One Rep Max)</h4>
    <p>
      A 1RM is the maximum amount of weight you can move doing an exercise.
      This calculator will give you a rough estimate of the maximum weight you can push/pull for any given exercise.
      <!-- <a href="https://vitejs.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>. -->
    </p>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

p {
  font-size: 1rem;
  padding: 1rem 0.5rem 1rem 0.5rem;
}

.greetings h1,
.greetings h3,
.greetings h4 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
