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
  font-size: 20px;
  margin: 25px auto;
  /* background: #24283b; */
  background: #1a1b26;
  padding: 25px;
  border-radius: 0.5em;
  box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.14),
    0px 2px 1px -1px rgba(0, 0, 0, 0.12), 0px 1px 3px 0px rgba(0, 0, 0, 0.2);
}

.card h3 {
  margin: 0;
}
</style>