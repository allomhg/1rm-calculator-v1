<script setup lang="ts">
// defineProps<{
//   msg: string
// }>()
</script>

<template>
  <div class="wrapper">
    <!-- <h1 class="green">{{ msg }}</h1> -->
    <h3>
      Select your units
    </h3>

    <!-- I could turn this radio button into its own component -->
    <div class="input-container">
      <div class="unit-select">
        <input type="radio" id="metric" name="units" value="metric" />
        <label for="metric">Metric (kg)</label>
      </div>
      <div class="unit-select">
        <input type="radio" id="imperial" name="units" value="imperial" />
        <label for="imperial">Imperial (lb)</label>
      </div>
    </div>

    <div class="input-container">
      <div class="unit-select">
        <label for="mass">Testies</label>
        <input type="number" id="mass" name="mass" value="mass" />
      </div>
      <div class="unit-select">
        <label for="reps">Reps:</label>
        <input type="number" id="reps" name="reps" value="reps" />
      </div>
    </div>

  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.wrapper {
  display: flex;
  flex-direction: column;
  background-color: grey;
  /* padding: -1rem; */
  border-radius: 0 0 1rem 1rem;
  align-items: center;
}

.input-container {
  display: inline-flex;
  background-color: red;
}

/* .unit-select {
} */

.wrapper h1,
.wrapper h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .wrapper h1,
  .wrapper h3 {
    text-align: left;
  }
}
</style>
