<script setup lang="ts">
import BandCardComponent from '@/components/findBand/BandCardComponent.vue';
import type { Band } from '@/models/band';

const DUMMY_DATA: Band[] = [
    {
        name: 'Big Joe Band',
        description: 'A band dedicated to making money and being swag.',
        genre: 'Blues',
    },
    {
        name: 'Keshi Cover Band',
        genre: 'Pop / RnB',
        description: 'We make covers of our fav Keshi songs!! :D',
        url: 'www.soundcloud.com/keshi',    
    },
    {
        name: 'Porter Robinson Fanboys',
        genre: 'Pop / EDM',
        description: `IT'S NOT FAAAAIIIIIIRR CUZ I KNOW YOU LIKE THE BACK OF MY HAND`
    }
]

const bands = DUMMY_DATA; //make API call
</script>

<template>
    <div>
        <BandCardComponent
            v-for="band in bands"
            :name="band.name"
            :genre="band.genre"
            :description="band.description"
            :url="band.url"
        />
    </div>
</template>