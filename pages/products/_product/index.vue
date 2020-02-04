<template>
  <div>
    <nuxt-child />
    <div>product id :{{ $route.params.product }}</div>
    <nuxt-link to="/"> Go home</nuxt-link>
  </div>
</template>

<script>
export default {
  validate(data) {
    return data.params.product == 1;
  }
};
</script>
