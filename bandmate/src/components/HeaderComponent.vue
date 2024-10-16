<script setup lang="ts">
import { RouterLink } from 'vue-router';
</script>

<template>
    <header>
        <h1>🎸 BandMate Page</h1>
        <RouterLink to="/" class="nav-link">Home</RouterLink>
        <RouterLink to="/about" class="nav-link">About</RouterLink>
        <RouterLink to="/find" class="nav-link">Find</RouterLink>
        <RouterLink to="/post" class="nav-link">Post</RouterLink>
    </header>
</template>

<style scoped>
h1 {
    display: inline;
    margin-right: 16px;
}

.nav-link {
    margin: 0px 8px;
    color: black;
    text-decoration: none;
} .nav-link:hover {
    text-decoration: underline;
}


</style>