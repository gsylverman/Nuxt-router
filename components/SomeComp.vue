<template>
  <div class="header">
    <ul class="nav-item">
      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/products">Contact</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.header {
  background: lightblue;
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: start;
  align-items: center;
}
.nav-item {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
}
li {
  padding: 25px;
}
li:hover {
  color: red;
}
</style>
