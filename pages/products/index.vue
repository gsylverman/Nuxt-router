<template>
  <div>
    products
    <input type="text" v-model="id" />
    <nuxt-link :to="`${$route.name}/${id}`">Go to product</nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: ""
    };
  }
};
</script>
