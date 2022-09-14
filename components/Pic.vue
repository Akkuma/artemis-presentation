<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps<{ src: string; imgclass?: string; imgstyle?: string }>()
</script>
<template>
<figure>
    <img
        :src="src"
        :class="imgclass"
        :style="imgstyle"
        class="relative rounded-full object-cover w-70px h-70px border border-4 border-secondary-400 z-10"
    />
</figure>
</template>