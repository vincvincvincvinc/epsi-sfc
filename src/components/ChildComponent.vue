<script>
export default {
  props: {
    msg: String,
  },
  methods: {
    maMethodeLocale() {
      this.$emit("monEventPerso");
    },
  },
};
</script>

<template>
  <div>
    <p>Received message from parent: {{ msg }}</p>
    <button @click="maMethodeLocale">Click me!</button>
  </div>
</template>

<style scoped>

</style>