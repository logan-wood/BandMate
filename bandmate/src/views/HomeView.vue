<script setup>
import GenreComponent from '@/components/home/GenreComponent.vue';

const GENRES = ['Rock', 'Pop', 'Blues']
</script>

<template>
  <div>
    <h1>🎸 BandMate Page</h1>
    <a href="about">About</a>

    <GenreComponent 
    v-for="genre in GENRES"
    :genre="genre"
    />
  </div>
</template>
