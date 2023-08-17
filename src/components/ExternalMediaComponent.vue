<script setup>
// import external logos
import GithubLogo from './icons/GitubLogo.vue';
import LinkedInLogo from './icons/LinkedInLogo.vue';
import EnvelopeLogo from './icons/EnvelopeLogo.vue';
</script>

<template>
    <div class="external-media">
      <a href="https://github.com/nmorrish" target="_blank"><GithubLogo/></a>
      <a href="https://www.linkedin.com/in/nicholas-morrish/" target="_blank"><LinkedInLogo/></a>
      <a href="mailto:nick.morrish@m-is.net" target="_blank"><EnvelopeLogo/></a>
    </div>
</template>
<style scoped>
    .external-media a{
        margin:0 0.5rem;
    }

    .external-media{
        display: flex;
        justify-content: center;
    }

    .external-media svg{
        height: 2rem;
    }
</style>