<template>
  <carousel :items-to-show="1">
    <slide v-for="post in posts" :key="post.id">
      <img class="slide-image" :src="post.image" alt="slide.title" />
      <div class="slide-content">
        <h2>{{ post.title }}</h2>
        <p>{{ post.description }}</p>
      </div>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
</template>

<script setup>
import 'vue3-carousel/dist/carousel.css'
import {Carousel, Slide, Pagination, Navigation} from 'vue3-carousel'

// get posts from props
const props = defineProps({
  posts: {
    type: Array,
    required: true,
  }
})
</script>

<style scoped lang="scss">
// the text should be over the image on the bottom and should have a background
.slide-content {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: 1rem;
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
}
</style>