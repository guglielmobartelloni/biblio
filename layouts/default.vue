<template>
  <div>
    <div class="container">
      <header class="blog-header py-3">
        <div class="row flex-nowrap justify-content-between align-items-center">
          <div class="col-4 pt-1">
            <nuxt-link class="text-muted" to="/"><b>Home</b></nuxt-link>
          </div>
          <div class="col-4 text-center">
            <nuxt-link class="blog-header-logo text-dark" to="/"
              >Gruppo San Giorgio</nuxt-link
            >
          </div>
          <div class="col-4 d-flex justify-content-end align-items-center">
            <!-- <a class="text-muted" href="#"> -->
            <!-- <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="mx-3"><circle cx="10.5" cy="10.5" r="7.5"></circle><line x1="21" y1="21" x2="15.8" y2="15.8"></line></svg> -->
            <!-- </a> -->
            <nuxt-link class="btn btn-sm btn-outline-secondary mr-2" to="/eventi"
              >Eventi</nuxt-link
            >
            <nuxt-link class="btn btn-sm btn-outline-secondary" to="/contatti"
              >Contatti</nuxt-link
            >
          </div>
        </div>
      </header>
      <Nuxt />
    </div>
    <footer class="text-center text-lg-start bg-light text-muted mt-4">
      <div
        class="text-center p-4"
        style="background-color: rgba(0, 0, 0, 0.05)"
      >
        © 2022 Copyright:
        <a class="text-reset fw-bold" href="#">Guglielmo Bartelloni</a>
      </div>
    </footer>
  </div>
</template>