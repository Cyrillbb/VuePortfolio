<template>
  <div class="card">
    <slot></slot>
  </div>
</template>

<script>
export default {};
</script>

<style>
.card {
  max-width: 600px;
  /* margin: 0 auto; */
  font-size: 20px;
  margin: 45px auto;
  background: #24283b;
  padding: 25px;
  border-radius: 0.5em;
}
</style>