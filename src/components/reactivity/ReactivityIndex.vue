<script setup lang="ts">
import CounterWithRef from "@/components/reactivity/CounterWithRef.vue";
import CounterWithReactive from "@/components/reactivity/CounterWithReactive.vue";
</script>

<template>
  <div class="container mt-3">
    <div class="row">
      <div class="col-md-6">
        <CounterWithRef/>
      </div>
      <div class="col-md-6">
        <CounterWithReactive/>
      </div>
    </div>
  </div>
</template>