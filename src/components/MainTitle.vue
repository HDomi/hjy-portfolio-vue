<script setup lang="ts">
defineProps<{
  maintit: string
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ maintit }}</h1>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 1.8rem;
  top: -10px;
}

.greetings h1{
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1{
    text-align: left;
  }
}
</style>
