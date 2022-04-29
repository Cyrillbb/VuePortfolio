<template>
  <div class="card">
    <div class="card-header">
      <slot name="card-header"></slot>
    </div>
    <div class="card-body">
      <slot name="card-body"></slot>
    </div>
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
  padding: 0 25px 25px;
  border-radius: 0.5em;
  box-shadow: 0px 1px 1px 0px rgb(0 0 0 / 14%),
    0px 2px 1px -1px rgb(0 0 0 / 12%), 0px 1px 3px 0px rgb(0 0 0 / 20%);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.card-header {
  /* background: #414868; */
  background: #5a4a78;
  text-align: center;
  width: 125%;
  padding: 5px 0;
  margin-bottom: 10px;
}
</style>