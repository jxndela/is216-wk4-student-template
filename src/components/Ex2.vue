<script setup>
    import { ref } from 'vue'

    // Add code here
    // static import of images - meaning the images are imported at build time and bundled with the application
    import wad from '/public/assets/wad.png'
    // reactive import of images - meaning the images are imported at runtime and can be changed dynamically
    const me = ref('/public/assets/me.png')
</script>

<template>

    <!-- Add code here -->
    <!-- v-bind used to bind the src attribute of the img tag to a reactive variable -->
    <img v-bind:src="wad" alt="wad" width="200" height="200">
    <img v-bind:src="me" alt="me" width="200" height="200">
</template>
