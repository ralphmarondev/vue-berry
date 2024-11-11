<script setup lang="ts">
import {ref, watch} from "vue";

const question = ref('')
const answer = ref('Question usually contain a question mark. :)')
const loading = ref(false)

watch(question, async (newQuestion, oldQuestion) => {
  console.log(`Old question: ${oldQuestion}`)
  if (newQuestion.includes('?')) {
    loading.value = true
    answer.value = 'Thinking...'

    try {
      const res = await fetch('https://localhost:8080/api')
      answer.value = (await res.json()).answer
    } catch (error) {
      answer.value = 'Error! Could not reach the API. ' + error
    } finally {
      {
        loading.value = false
      }
    }
  }
})
</script>

<template>
  <div class="container mt-3">
    <div class="card shadow">
      <div class="card-content">
        <h3 class="card-header">Basic Watcher</h3>
        <div class="card-body">
          <p>Ask a yes/not question:</p>
          <input type="text" v-model="question" :disabled="loading" class="form-control">
        <p>{{ answer}}</p>
        </div>
      </div>
    </div>
  </div>
</template>