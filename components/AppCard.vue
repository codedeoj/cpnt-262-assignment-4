<script setup>
  // defineProps({
  //   title: {
  //     type: String,
  //     default: "Card Title"
  //   },
  //   description: {
  //     type: String,
  //     default: "Card Description"
  //   },
  // })

  defineProps({
    info: {
      type: Object,
      default() {
        return {
          title: "Card Title",
          description: "Card Description"
        };
      },
    },
    link: {
      type: Object,
      default() {
        return {
          url: "#",
          text: "Explore",
        };
      },
    },
  })
</script>

<template>
  <article class="max-w-sm rounded shadow-lg mx-auto my-8 px-6 py-4">
    <div>
      <h3 class="text-lg font-semibold mb-2">{{ info.title }}</h3>
    </div>
    <div>
      <p>{{ info.description }}</p>
    </div>
    <div>
      <NuxtLink :to="link.url" class="inline-block my-2 px-3 py-1 text-sm font-semibold bg-pink-500 hover:bg-pink-600 text-white">
        {{ link.text }}
      </NuxtLink>
    </div>
  </article>
</template>