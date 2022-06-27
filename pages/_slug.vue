<template>
  <div>
    <a to="/eventi" class="link-primary pointer" @click="$router.go(-1)"
      >Torna agli eventi</a
    >
    <nuxt-content :document="evento"></nuxt-content>
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const evento = await $content('eventi', params.slug)
      .sortBy('createdAt', 'desc')
      .fetch()

    return { evento }
  },
  methods: {
    formatDate(date) {
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return new Date(date).toLocaleDateString('it', options)
    },
  },
}
</script>

<style scoped>
.pointer {
  cursor: pointer;
}
</style>
