<template>
  <div class="container">
    <h1>Welcome to LoveZenVibe!</h1>

    <div class="row">
      <button class="lovea"  @click="emit('setView', 'love')">
        <img src="/love.png" class="logo loveb" alt="Love logo" />
        <h1 class="love">Love</h1>
      </button>
      <button class="zena" @click="emit('setView', 'zen')">
        <img src="/zen.png" class="logo zenb" alt="Zen logo" />
        <h1 class="zen">Zen</h1>
      </button>
      <button class="vibea"  @click="emit('setView', 'vibe')">
        <img src="/vibe.png" class="logo vibeb" alt="Vibe logo" />
        <h1 class="vibe">Vibe</h1>
      </button>
    </div>
    <p>Your Zen Garden of love zen and vibe!</p>
  </div>

  
</template>

<style scoped>


</style>

<script setup lang="ts">
const emit = defineEmits(['setView'])
</script>