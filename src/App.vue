<script setup lang="ts">
import HelloWorld from './components/ORMGreeting.vue'
// import TheWelcome from './components/TheWelcome.vue'
import RMInfo from './components/RMInfo.vue';
import InfoDisplay from './components/InfoDisplay.vue';
</script>

<template>
  <div class="content-wrapper">
    <header>
      <div class="wrapper">
        <HelloWorld msg="1RM Calculator" />
      </div>
    </header>

    <main>
      <!-- <TheWelcome /> -->
      <RMInfo />
      <InfoDisplay />
    </main>
  </div>
</template>

<style scoped>

header {
  line-height: 1.5;
}

.content-wrapper {
  border: solid 1px;
  border-radius: 1rem;
  /* padding: 1rem; */
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
