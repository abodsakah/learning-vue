<script setup>
import PostsCarousel from '../components/PostsCarousel.vue'


const posts = [
  {
    id: 1,
    title: 'Post 1',
    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec auctor, nisl eu ultricies aliquam, nisl libero ultricies urna, eget ultricies',
    image: 'https://picsum.photos/seed/picsum/200/300',
  },
  {
    id: 2,
    title: 'Post 2',
    description: 'Hello world',
    image: 'https://picsum.photos/seed/picsum/200/300',
  }
]

</script>

<template>
  <PostsCarousel :posts="posts" />
  <h1>Hello world</h1>
</template>