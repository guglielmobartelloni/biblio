<template>
  <div>
    <div class="px-4 my-5 text-center">
      <!-- <img class="d-block mx-auto mb-4" src="/docs/5.0/assets/brand/bootstrap-logo.svg" alt="" width="72" height="57"> -->
      <h1 class="display-5 fw-bold">Gruppo San Giorgio</h1>
      <div class="col-lg-6 mx-auto">
        <p class="lead mb-4">
          Quickly design and customize responsive mobile-first sites with
          Bootstrap, the world’s most popular front-end open source toolkit,
          featuring Sass variables and mixins, responsive grid system, extensive
          prebuilt components, and powerful JavaScript plugins.
        </p>
        <!-- <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
        <button type="button" class="btn btn-primary btn-lg px-4 gap-3">Primary button</button>
        <button type="button" class="btn btn-outline-secondary btn-lg px-4">Secondary</button>
      </div> -->
      </div>
    </div>

    <div class="row mb-2">
      <div class="col-md-6">
        <div class="card flex-md-row mb-4 box-shadow h-md-250">
          <div class="card-body d-flex flex-column align-items-start">
            <strong class="d-inline-block mb-2 text-primary">World</strong>
            <h3 class="mb-0">
              <a class="text-dark" href="#">Featured post</a>
            </h3>
            <div class="mb-1 text-muted">Nov 12</div>
            <p class="card-text mb-auto">
              This is a wider card with supporting text below as a natural
              lead-in to additional content.
            </p>
            <a href="#">Continue reading</a>
          </div>
          <img
            class="card-img-right flex-auto d-none d-md-block"
            data-src="holder.js/200x250?theme=thumb"
            alt="Card image cap"
          />
        </div>
      </div>
      <div class="col-md-6">
        <div class="card flex-md-row mb-4 box-shadow h-md-250">
          <div class="card-body d-flex flex-column align-items-start">
            <strong class="d-inline-block mb-2 text-success">Design</strong>
            <h3 class="mb-0">
              <a class="text-dark" href="#">Post title</a>
            </h3>
            <div class="mb-1 text-muted">Nov 11</div>
            <p class="card-text mb-auto">
              This is a wider card with supporting text below as a natural
              lead-in to additional content.
            </p>
            <a href="#">Continue reading</a>
          </div>
          <img
            class="card-img-right flex-auto d-none d-md-block"
            data-src="holder.js/200x250?theme=thumb"
            alt="Card image cap"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
