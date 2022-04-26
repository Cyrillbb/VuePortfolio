<template>
  <div class="app-header">
    <div>
      <span class="blue-text">#StandWith</span
      ><span class="yellow-text">Ukraine</span>
    </div>
    <div>
      <app-navigation></app-navigation>
    </div>
  </div>
</template>

<script>
import AppNavigation from "./AppNavigation.vue";
export default {
  components: {
    AppNavigation,
  },
};
</script>

<style>
.app-header {
  display: flex;
  justify-content: space-between;
}

.app-header > div {
  background: #24283b;
  width: max-content;
  padding: 20px;
  margin: 10px;
  font-size: 20px;
  border-radius: 0.5em;
}

.blue-text {
  color: #2ac3de;
}

.yellow-text {
  color: #e0af68;
}
</style>