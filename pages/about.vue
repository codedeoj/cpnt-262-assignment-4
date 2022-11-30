<template>
  <main>
    <PageHeader title="About Page"/>
    <AppSectionHeader title="About Me"/>
    <AboutSection />
    <AppButton class="mx-10">Contact Me</AppButton>
  </main>

  <!-- v-on example-->
  <p>v-on Example</p>
  <div class="text-center mt-20">
    <p>The Current Number is:</p>
    <h3 class="text-2xl">{{ number }}</h3>
    <button v-on:click="number++" class="text-xl font-bold mr-5">+</button>
    <button v-on:click="number--" class="text-xl font-bold ml-5">-</button>
  </div>
</template>

<script setup>
  const number = ref(0);
</script>