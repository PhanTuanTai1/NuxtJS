<template>
  <div class="col-md-6 ftco-animate">
    <div class="blog-entry">
      <a
        v-bind:href="href"
        class="img d-flex align-items-end"
        v-bind:style="'background-image: url(images/' + img + ')'"
      >
        <div class="overlay"></div>
      </a>
      <div class="text pt-3">
        <p class="meta d-flex">
          <span class="pr-3">{{subheading}}</span>
          <span class="ml-auto pl-3">March 01, 2018</span>
        </p>
        <h3>
          <a v-bind:href="href">{{topic}}</a>
        </h3>
        <p class="mb-0">
          <a v-bind:href="href" class="btn-custom">
            Read More
            <span class="icon-arrow_forward ml-4"></span>
          </a>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["subheading", "topic", "href", "img"],
};
</script>