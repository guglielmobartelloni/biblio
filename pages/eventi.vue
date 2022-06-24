<template>
  <div>
    <!-- <div v-for="evento in eventi" :key="evento.title">
      <nuxt-content  :document="evento" />
</div> -->
    <div>
      <main role="main" class="container">
        <div class="row">
          <div class="col-12 blog-main">
            <h3 class="pb-3 mb-4 font-italic border-bottom">Eventi</h3>
            <div v-for="evento in eventi" :key="evento.title" class="border-bottom">
              <div class="blog-post">
                <h2 class="blog-post-title">{{ evento.title }}</h2>
                <p class="blog-post-meta">
                  January 1, 2014 by <a href="#">Mark</a>
                </p>
               <nuxt-content :document="evento" />
              </div>
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
    const eventi = await $content('eventi')
      .sortBy('createdAt', 'desc')
      .fetch()

    return { eventi }
  },
}
</script>
