<script setup>
//import external media links
import MediaLinks from '../components/ExternalMediaComponent.vue'
</script>

<template>
    <div class="footer-container">
        <MediaLinks/>
        <p>&copy; Nick Morrish 2023</p>
    </div>
    
</template>

<style scoped>
    .footer-container{
        text-align: center;
        padding-bottom: 3rem;
    }
    p{
        padding-top: 0.5rem;
    }
</style>