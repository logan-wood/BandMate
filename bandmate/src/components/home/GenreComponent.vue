<script setup lang="ts">
import { defineProps } from 'vue';

const props = defineProps({ genre: String })
</script>

<template>
    <div>
        <h4>{{ props.genre }}</h4>
    </div>
</template>

<style scoped>
div {
    margin: 16px;
    padding: 16px;
    border: 1px solid black;
    border-radius: 16px;
} div:hover {
    cursor: pointer;
}

h4 {
    text-align: center;
}
</style>