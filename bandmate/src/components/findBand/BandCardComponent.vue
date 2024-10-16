<script setup lang="ts">
import { defineProps } from 'vue';
import type { Band } from '@/models/band';

const props = defineProps<Band>();
</script>

<template>
    <div>
        <h4>{{ props.name }}</h4>
        <p>{{ props.description }}</p>
        <p>{{ props.genre }}</p>
    </div>
</template>