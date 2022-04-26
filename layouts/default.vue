<template>
  <div class="default-layout">
    <app-header></app-header>
    <nuxt></nuxt>
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader.vue";
export default {
  components: { AppHeader },
};
</script>

<style>
</style>