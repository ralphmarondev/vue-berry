<script setup lang="ts">

import {computed, reactive} from "vue";

const developer = reactive({
  name: 'Ralph Maron Eda',
  projects: [
    'Family Sprout - Version 1.2 is released 2 months ago',
    'Compose World - On Progress',
    'Taskify - To be updated.',
    'Photo Diary - Will continue later.',
    'Maron OS - Haven\'t touched for months.'
  ]
})

// returns ref
const projectsMessage = computed(() => {
  return developer.projects.length > 0 ? 'Yes' : 'No'
})
</script>

<template>
  <div class="card shadow">
    <div class="card-content text-center">
      <h3 class="card-header">Computed Caching</h3>
      <div class="card-body">
        <p class="text-primary">Has projects:</p>
        <span class="text-secondary">{{ projectsMessage}}</span>
      </div>
    </div>
  </div>
</template>