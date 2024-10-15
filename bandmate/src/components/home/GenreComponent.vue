<script setup>
import { defineProps } from 'vue';

const props = defineProps({ genre: String })
</script>

<template>
    <div>
        <h4>{{ props.genre }}</h4>
    </div>
</template>