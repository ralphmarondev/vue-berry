<script setup lang="ts">
import {ref} from "vue";

const choice = ref(0)
const isEven = () => {
  return choice.value > 0 && choice.value % 2 === 0
}
const isOdd = () => {
  return choice.value > 0 && choice.value % 2 !== 0
}
const isZero = () => {
  return choice.value === 0
}
</script>

<template>
  <div class="container mt-3">
    <div class="row">
      <div class="col-md-6">
        <div class="card shadow">
          <div class="card-content">
            <h3 class="card-header">Conditional Rendering</h3>
            <div class="card-body">
              <div class="row mb-3 px-3">
                <label for="choice" class="form-label">Choice</label>
                <input type="text" name="choice" class="form-control" placeholder="Enter Choice" v-model="choice">
              </div>

              <h3 v-if="isZero()">Hello, Zero</h3>
              <h3 v-else-if="isEven()">Hello, Even</h3>
              <h3 v-else-if="isOdd()">Hello, Odd</h3>
              <h3 v-else>Hello, Negative</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>