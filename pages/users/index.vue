<template>
  <div>
    users
    <input type="text" v-model="id" />
    <button @click="setUser">set user</button>
    <nuxt-link :to="`${$route.name}/${id}`">users</nuxt-link>
  </div>
</template>

<script>
export default {
  created() {
    console.log(this.$route);
  },
  data() {
    return {
      id: "",
      link: "google.com"
    };
  },
  methods: {
    setUser() {
      this.$router.push("/users/" + this.id);
    }
  },
  computed: {
    d() {
      return this.link;
    }
  }
};
</script>
