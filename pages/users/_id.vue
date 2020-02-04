<template>
  <div>
    <div>User id: {{ $route.params.id }}</div>
    <button @click="$router.push('/')">Home</button>
  </div>
</template>

<script>
export default {
  methods: {}
};
</script>
