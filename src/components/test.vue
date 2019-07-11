<template>
  <carousel :navigationEnabled="true" :centerMode="true" :paginationEnabled="false" :perPage="5" :spacePadding="10">
      <slide v-for="value in data">
        <div class="item-style">
          <a :href="value.path">
            <h2>{{ value.name }}</h2>
          </a>
        </div>
      </slide>
  </carousel>
</template>

<script>
  import { Carousel, Slide } from 'vue-carousel';

  export default {
    name: 'test',
    components: {
      carousel: Carousel,
      slide: Slide,
    },
    props: ['data'],
  };
</script>

<style>
  .VueCarousel {
    width: 80%;
    margin: 0 auto;
  }

</style>
