<template>
  <div class="navbar-container">
    <a href="/"><h1>Abod's blog</h1></a>

    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/blog">Blog</router-link>
      <router-link to="/about">About</router-link>
    </nav>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
  .navbar-container {
    width: 100%;
    min-height: 10%;
    border-bottom: 1px solid #4d4d4d;
    background-color: var(--color-background-soft);
    display: flex;
    justify-content: space-evenly;
    align-items: center;

    a {
      text-decoration: none;
    }

    nav {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-left: 2rem;
      font-size: 1.5rem;
      font-weight: 500;

      a {
        margin-left: 2rem;
        color: var(--color-text);
      }
    }
  }
</style>