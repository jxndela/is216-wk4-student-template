<script setup>
    import { ref } from 'vue'

    // Add code here
    // In Ex3.vue, a dropdown list is provided to allow users to login with either
    // username or email. Render the page different depending on the
    // selection, i.e., show an input for an email or a username accordingly.
    // Hint: use v-model, v-if, and v-else to accomplish the task

    const loginOption = ref('username')
    
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <select v-model="loginOption">
        <option value="username" selected>Username login</option>
        <option value="email">Email login</option>
    </select>
    
    <div v-if="loginOption === 'username'">
        <label>Username</label>
        <input placeholder="Enter your username">
    </div>
    <div v-else="loginOption === 'email'">
        <label>Email</label>
        <input placeholder="Enter your email">
    </div>
</template>

