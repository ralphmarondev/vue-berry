<script setup lang="ts">
import {reactive} from "vue";

const state = reactive({count: 0})
const increment = () => {
  state.count++
}
const decrement = () => {
  state.count--
}

</script>

<template>
  <div class="card shadow">
    <div class="card-content text-center">
      <h3 class="card-header">Counter - Reactive</h3>
      <div class="card-body">
        <p class="text-primary">Count: {{ state.count }}</p>
        <div class="row">
          <div class="col">
            <button @click="increment" type="button" class="btn btn-primary">Increment</button>
          </div>
          <div class="col">
            <button @click="decrement" type="button" class="btn btn-secondary">Decrement</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>