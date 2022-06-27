<template>
  <div class="card">
    <img class="card-img-top" :src="require(`~/assets/images/${img}`)" />
    <div class="card-body">
      <nuxt-link
        class="card-title"
        :to="{ name: 'slug', params: { slug: slug } }"
        >{{ title }}</nuxt-link
      >
      <p class="card-text">{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
    description: {
      type: String,
      required: true,
    },
    img: {
      type: String,
      required: true,
    },
    slug: {
      type: String,
      required: true,
    },
  },
}
</script>
