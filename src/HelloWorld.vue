<script setup lang="ts">

interface ButtonProps {
    border?: boolean; 
}

const props = defineProps<ButtonProps>() 
defineEmits<{
    (event: 'click',payload: MouseEvent): void
}>()
</script>
<template>
    <div id="app">
        <button @click="$emit('click', $event)">Click me</button>
    </div>
</template>