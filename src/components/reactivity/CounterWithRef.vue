<script setup lang="ts">
import {ref} from "vue";

const count = ref(0)
const increment = () => {
  count.value++
}
const decrement = () => {
  count.value--
}

</script>

<template>
  <div class="card shadow">
    <div class="card-content text-center">
      <h3 class="card-header">Counter - Ref</h3>
      <div class="card-body">
        <p class="text-primary">Count: {{ count }}</p>
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