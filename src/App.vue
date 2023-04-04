<script setup>
  import { RouterLink, RouterView } from 'vue-router'
  import Header from './components/Header.vue'
  import Footer from './components/Footer.vue'
</script>
<template>
  <header>
    <Header/>
    <nav>
        <RouterLink to="/">About Me</RouterLink>
        <RouterLink to="/projects">My projects</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>
  </header>
  <hr class="section-break">
  <main>
    <!-- <Body /> -->
    <RouterView />
  </main>
  <hr class="section-break">
  <footer>
    <Footer />
  </footer>
</template>

<style scoped>
  nav{
    display:flex;
    justify-content: center;
    column-gap: 3rem;
    margin-top:2rem;
    font-size:1.8rem;
  }

  nav a.router-link-exact-active {
    color: var(--primary-font-color);
    transition: color 0.5s;
  }
</style>
