<script setup>
import { RouterLink } from 'vue-router';
</script>

<template>
    <div>

        <!-- Doing this will refresh the page, so, its bad with states (ref) -->
        <!-- <a href="/">Home</a>
        <a href="/about">About</a> -->

        <!-- use RouterLink to visit outer route without affecting the states -->
        <RouterLink active-class="active" to="/">Home</RouterLink>
        <RouterLink active-class="active" to="/about">About</RouterLink>

        <!-- this link doesn't exist, but we will go to it -->
        <!-- active class does not work on here -->
        <RouterLink active-class="active" to="/xxx">About</RouterLink>

        <!-- active-class: is the class to use when that page is active -->
    </div>
</template>

<style scoped>
.active {
    color: red;
}
</style>