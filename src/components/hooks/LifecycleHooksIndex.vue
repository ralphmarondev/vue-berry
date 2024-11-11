<script setup lang="ts">
import {onMounted} from "vue";

onMounted(() => {
  console.log("Component mounted.")
})
</script>

<template>
  <div class="container mt-3">
    <div class="card shadow">
      <div class="card-content">
        <h3 class="card-header">Registering Lifecycle Hooks</h3>
        <div class="card-body">
          Open console and see that it is mounted already.
        </div>
      </div>
    </div>
  </div>
</template>