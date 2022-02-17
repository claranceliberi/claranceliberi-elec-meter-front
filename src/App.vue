<script setup lang="ts">
  import {ref } from 'vue'
  import BuyToken from './components/BuyToken.vue'
  import LoadToken from './components/LoadToken.vue'
  import TokenInfo from './components/TokenInfo.vue'

  const tab = ref(1)

</script>

<template>
  <div class="menu">
    <ul>
      <li @click="tab = 1">Info</li>
      <li @click="tab = 2">Load</li>
      <li @click="tab = 3">Buy</li>
    </ul>
  </div>
  <div class="tabs">
    <div class="load" v-if="tab === 2 "> <LoadToken/> </div>
    <div class="buy" v-else-if="tab === 3">
      <BuyToken />
    </div>
    <div class="info" v-else>
      <TokenInfo />
    </div>
  </div>
</template>

<style>

</style>
