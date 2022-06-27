<template>
  <div>
    <nuxt-link to="/eventi">Torna agli eventi</nuxt-link>
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
