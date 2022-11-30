<script setup>
  const cards = [
    {
      info: {
        title: "UI/UX Designer",
        description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis ipsum error eligendi molestiae eaque quas, ducimus sequi excepturi?"
      },
   },
   {
      info: {
        title: "Web Development",
        description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis ipsum error eligendi molestiae eaque quas, ducimus sequi excepturi?"
      },
  },
  {
      info: {
        title: "Brand & Logo Design",
        description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis ipsum error eligendi molestiae eaque quas, ducimus sequi excepturi?"
    },
  },
  {
    info: {
      title: "Web Design",
      description: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis ipsum error eligendi molestiae eaque quas, ducimus sequi excepturi?"
    },
  }
  ]
</script>

<template>
  <main>
    <PageHeader title="Home Page"/>
    <AppSectionHeader title="My Services"/>
    <CardLayout>
    <AppCard 
      v-for="card in cards"
      :key="card.id"
      :info="card.info"
    />
    </CardLayout>
    <AppButton class="text-center">Learn More...</AppButton>
  </main>
</template>