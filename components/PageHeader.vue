<script setup>
  defineProps({
    title: {
      type: String,
    }
  })
</script>

<template>
  <header class="flex justify-center font-bold text-3xl my-5">
    <h1>
      {{ title }}
    </h1>
  </header>
</template>