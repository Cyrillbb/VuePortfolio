<template>
  <div>
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
