<script setup lang="ts">
    import { ref } from 'vue'
    
    const token = ref("")
</script>

<template>
    <form>
        <label for="token">
            <span>token</span>
            <input v-model="token" type="text" id="token">
        </label>
        <button type="submit">Load</button>
    </form>
</template>