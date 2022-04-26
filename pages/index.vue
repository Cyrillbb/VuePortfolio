<template>
  <div>
    <div class="main-page-header">
      <div class="text-big">Hello, My name is Cyill Baryshnikov</div>
      <div class="text-big text-darker">
        And I'm a <span class="text-neon">passionate</span> front-end developer
      </div>
    </div>
    <app-tag-cloud></app-tag-cloud>
  </div>
</template>

<script>
import AppShortSummary from "../components/AppShortSummary.vue";
import AppTagCloud from "../components/AppTagCloud.vue";
export default {
  components: { AppTagCloud, AppShortSummary },
};
</script>

<style>
.main-page-header {
  /* position: absolute; */
  margin: 100px 0 0 130px;
}
</style>