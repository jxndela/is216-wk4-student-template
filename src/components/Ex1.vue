<script setup>
    import { ref } from 'vue'

    // Add code here
    // challenge: use array  
    // ref with array of fruits and use v-for to display them in the template
    const fruits = ref(['apple', 'orange', 'peach'])
    const message = ref('Choose your favorite fruit:')
</script>

<template>
    {{ message }} 

    <label for=""> <input type="radio" name="fruit"> {{ fruits[0] }} </label> 
    <label for=""> <input type="radio" name="fruit"> {{ fruits[1] }} </label> 
    <label for=""><input type="radio" name="fruit"> {{ fruits[2] }} </label> 
    
</template>

<style scoped>
</style>
