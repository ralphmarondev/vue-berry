<script setup lang="ts">
import {reactive, ref} from "vue";

const isActive = ref(false)
const hasError = ref(true)

// with reactive
const classObject = reactive({
  active: true,
  'text-danger': false
})
</script>

<template>
  <div class="card shadow">
    <div class="card-content">
      <h3 class="card-header">Binding to Objects</h3>
      <div class="card-body">
        <p class="static" :class="{active: isActive, 'text-danger': hasError}">Hello, Ralph Maron Eda is here!</p>
        <p class="static" :class="classObject">Hello, Ralph Maron Eda is here!</p>
      </div>
    </div>
  </div>
</template>