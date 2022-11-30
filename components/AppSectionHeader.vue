<script setup>
defineProps({
  title: String,
});
</script>
<template>
  <header class="text-2xl font-semibold text-center underline mt-10">
    <h2>{{ title }}</h2>
  </header>
</template>