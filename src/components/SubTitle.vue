<script setup lang="ts">
    defineProps<{
        subtit: string
}>()
</script>

<template>
    <div class="greetings">
      <h3>{{ subtit }}</h3>        
    </div>
  </template>


<style scoped>
    h3 {
      font-size: 1.2rem;
    }
    .greetings h3 {
      text-align: center;
    }
    
    @media (min-width: 1024px) {
      .greetings h3 {
        text-align: left;
      }
    }
    </style>
    