<!-- views/HomeView.vue -->
<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="text-3xl font-bold">
    <h1 class="">{{ msg }}</h1>
  </div>
</template>
