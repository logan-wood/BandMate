<script setup>
import GenreComponent from '@/components/home/GenreComponent.vue';

const GENRES = ['Rock', 'Pop', 'Alternative', 'Acoustic', 'Blues', 'Electronic', 'Hip-Hop', 'Country', 'Metal']
</script>

<template>
  <div class="genre-grid">
    <GenreComponent 
    v-for="genre in GENRES"
    :genre="genre"
    />
  </div>
</template>

<style>
.genre-grid {
  display: grid;
  grid-template-columns: auto auto auto;
  margin: 0 auto;
  width: 80%;
}
</style>
