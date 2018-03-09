<template>
<v-layout>
  <v-flex>
    <h1>Home Page</h1>
  </v-flex>
</v-layout>
</template>

<script>

export default {
  async asyncData({ app }) {
    const call = await app.$axios.$get('http://localhost:3000')
    return { call }
  },
  components: {

  }
}
</script>

<style>

</style>
