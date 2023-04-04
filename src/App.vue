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
    
    <router-view v-slot="{ Component }">
      <transition name="scale">
        <component :is="Component" />
      </transition>
    </router-view>
  </main>
  <hr class="section-break">
  <footer>
    <Footer />
  </footer>
</template>

<style scoped>

  .scale-enter-active,
  .scale-leave-active {
    transition: all 0.5s ease;
  }
  .scale-enter-from,
  .scale-leave-to {
    opacity: 0;
    transform: scale(0.9);
  }

  .scale-leave-active.scale-leave-to{
    display: none;
  }

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
