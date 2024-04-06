<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import {ref }from "vue";
import Love from "./components/Love.vue";

import Zen from "./components/Zen.vue";

import Vibe from "./components/Vibe.vue";
import ZenGarden from "./components/ZenGarden.vue";

import NavBar from "./components/NavBar.vue";

import AppBar from "./components/AppBar.vue";
const CurrentView = ref("home");

function setView(view:string){
    CurrentView.value = view;
}

</script>

<template>
  <!-- <button @click="setView('home')">Home</button>
  
  <button @click="setView('love')">Love</button> -->
  <AppBar />
  <div class="App">
    <NavBar @setView="setView" v-if="CurrentView!='home'"/>
    <ZenGarden @setView="setView" v-if="CurrentView=='home'"/>
    <Vibe v-if="CurrentView=='vibe'"/>
    <Zen v-if="CurrentView=='zen'"/>
    <Love v-if="CurrentView=='love'"/>
  </div>
</template>

<style scoped>

</style>
