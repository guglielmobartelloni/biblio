<template>
<div>
  <!-- <div v-for="evento in eventi" :key="evento.title">
      <nuxt-content  :document="evento" />
</div> -->
  <div>
    <h1 class="text-7xl font-black text-center">Eventi</h1>
    <div v-for="evento in eventi" :key="evento.title">
      <h2 class="mt-2 text-3xl font-semibold">{{ evento.title }}</h2>
    </div>
  </div>
</div>
</template>

<script>
  export default {
    async asyncData({ $content, params }) {
      const eventi = await $content('eventi')
      .only(['title', 'image', 'tags', 'slug'])
      .sortBy('createdAt', 'desc')
      .fetch()

      return {eventi}
    }
  }
</script>
