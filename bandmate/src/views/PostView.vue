<script setup lang="ts">
import type { Band } from '@/models/band';
import { ref } from 'vue';

var newBand = ref<Band>({
    name: '',
    description: '',
    genre: '',
});

function submitPost() {
    console.log('To be implemented');
}

</script>

<template>
    <div>
        <h1>Create Post</h1>

        <label for="name">Band Name</label><br>
        <input v-model="newBand.name" placeholder="Band Name" />

        <br>
        <label for="genre">Genre</label><br>
        <input v-model="newBand.genre" placeholder="Genre" />

        <br>
        <label for="desc">Description</label><br>
        <input v-model="newBand.description" placeholder="Description" />

        <br>
        <label for="url">URL</label><br>
        <input v-model="newBand.url" placeholder="Socials" />

        <br>
        <button onclick="submitPost()">Submit</button>

    </div>
</template>