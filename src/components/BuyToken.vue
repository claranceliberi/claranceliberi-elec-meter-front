<script setup lang="ts">
    import { reactive } from 'vue'
    
    const token = reactive({
        meter:'',
        ammount:''
    })
</script>

<template>
    <form>
        <label for="meter">
            <span>Meter</span>
            <input v-model="token.meter" type="text" id="meter">
        </label>
        <label for="ammount">
            <span>Ammount</span>
            <input v-model="token.ammount" type="text" id="ammount">
        </label>
        <button type="submit">Purchase</button>
    </form>
</template>