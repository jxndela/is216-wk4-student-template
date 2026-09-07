<script setup>
    import { ref } from 'vue'

    // Add code here
    import wad from '/public/assets/wad.png'
    const me = ref('/public/assets/me.png')
</script>

<template>

    <!-- Add code here -->
    <img :src="wad" alt="wad" width="200" height="200">
    <img :src="me" alt="me" width="200" height="200">
</template>
