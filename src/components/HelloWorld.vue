<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>
  <div class="card">
    <button type="button" @wheel="count++" @click="count--">
      count is {{ count }}
    </button>
    <p>Edit <code>components/HelloWorld!.vue</code> to test HMR</p>
  </div>
</template>
