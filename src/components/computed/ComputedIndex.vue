<script setup lang="ts">
import ComputedCaching from "@/components/computed/ComputedCaching.vue";
import WritableComputed from "@/components/computed/WritableComputed.vue";
</script>

<template>
  <div class="container mt-3">
    <div class="row">
      <div class="col-md-6">
        <ComputedCaching/>
      </div>
      <div class="col-md-6">
        <WritableComputed/>
      </div>
    </div>
  </div>
</template>