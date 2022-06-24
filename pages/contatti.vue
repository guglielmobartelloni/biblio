<template>
  <form name="contact" method="POST" data-netlify="true" action="/grazie" data-netlify-honeypot="bot-field">
    <input type="hidden" name="form-name" value="contact" />

    <!-- Name input -->
    <div class="form-outline mb-4">
      <label class="form-label">Nome e Congnome </label>
      <input type="text" name="fullname" class="form-control" />
    </div>

    <!-- Email input -->
    <div class="form-outline mb-4">
      <label class="form-label" for="form4Example2">Indirizzo Email </label>
      <input type="email" name="email" class="form-control" />
    </div>

    <!-- Note input -->
    <div class="form-outline mb-4">
      <label class="form-label" for="form4Example3">Note </label>
      <textarea class="form-control" name="note" rows="4"> </textarea>
    </div>

    <!--
      <\!-- Checkbox -\-> -->
    <!--
      <div class="form-check d-flex justify-content-center mb-4"> -->
    <!--
      <input class="form-check-input me-2" type="checkbox" value="" id="form4Example4" checked /> -->
    <!--
      <label class="form-check-label" for="form4Example4"> -->
    <!--     Send me a copy of this message -->
    <!--
      </label> -->
    <!--
      </div> -->

    <!-- Submit button -->
    <button type="submit" class="btn btn-primary btn-block mb-4">Invia</button>
  </form>
</template>