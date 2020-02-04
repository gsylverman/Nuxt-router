<template>
  <div>
    <input type="text" v-model="id" />
    <button @click="goTo">Load user</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: ""
    };
  },
  methods: {
    goTo() {
      this.$router.push("/users/" + this.id);
    }
  }
};
</script>
