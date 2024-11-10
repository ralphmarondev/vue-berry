<script setup lang="ts">

import {computed, ref} from "vue";

const firstName = ref('Ralph Maron')
const lastName = ref('Eda')

const fullName = computed({
  get() {
    return `${firstName.value} ${lastName.value}`
  },
  set(newValue) {
    [firstName.value, lastName.value] = newValue
  }
})
</script>

<template>
  <div class="card shadow">
    <div class="card-content">
      <h3 class="card-header text-center">Writable Computed</h3>
      <div class="card-body">
        <form class="px-3">
          <div class="row mb-3">
            <label for="first-name" class="form-label">First Name</label>
            <input type="text" class="form-control" v-model="firstName" placeholder="First Name">
          </div>
          <div class="row mb-3">
            <label for="last-name" class="form-label">Last Name</label>
            <input type="text" class="form-control" v-model="lastName" placeholder="Last Name">
          </div>
          <button type="submit" class="btn btn-primary mb-3">
            Submit
          </button>
          <p class="text-secondary">{{fullName}}</p>
        </form>
      </div>
    </div>
  </div>
</template>