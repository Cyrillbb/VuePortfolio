<template>
  <ul class="app-nav-ul">
    <li>
      <nuxt-link to="/">Home</nuxt-link>
    </li>
    <li>
      <nuxt-link to="/experiences/">About</nuxt-link>
    </li>
  </ul>
</template>

<script>
export default {};
</script>

<style>
.app-nav-ul {
    display: flex;
    list-style: none;
    margin: 0;
}
</style>