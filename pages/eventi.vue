<template>
  <div>
    <!-- <div v-for="evento in eventi" :key="evento.title">
      <nuxt-content  :document="evento" />
</div> -->
    <div>
      <main role="main" class="container">
        <div class="row">
          <div class="col-12 blog-main">
            <h3 class="pb-3 mb-4 font-bold border-bottom">Eventi</h3>
            <div class="card-columns">
                <EventsCard
                  v-for="evento in eventi"
                  :key="evento.title"
                  :description="evento.description"
                  :title="evento.title"
                  :img="evento.img"
                  :slug="evento.slug"
                />
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const eventi = await $content('eventi').sortBy('createdAt', 'desc').fetch()
    return { eventi }
  },
  methods: {
    formatDate(date) {
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return new Date(date).toLocaleDateString('it', options)
    },
  },
}
</script>
