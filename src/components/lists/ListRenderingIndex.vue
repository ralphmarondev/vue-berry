<script setup lang="ts">

import {ref} from "vue";

const items = ref([{id: 0, message: 'Hi'}, {id: 1, message: 'Hello'}])
</script>

<template>
  <div class="container mt-3">
    <div class="card shadow">
      <div class="card-content">
        <h3 class="card-header">List Rendering</h3>
        <div class="card-body">
          <li v-for="item in items" :key="item.id" class="list-unstyled">
            <span class="text-secondary"> {{ item.message }}</span>
          </li>
        </div>
      </div>
    </div>
  </div>
</template>