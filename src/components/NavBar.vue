<script setup lang="ts">
  /* import { ref } from "vue";
  import { invoke } from "@tauri-apps/api/tauri";

  const love = ref(""); */
  const emit = defineEmits(['setView'])
</script>

<template>
  <a href="#" @click="emit('setView', 'home')"><h1>Home</h1></a>
</template>