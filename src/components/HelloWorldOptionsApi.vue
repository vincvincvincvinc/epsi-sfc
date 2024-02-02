<script>
export default {
  name: "HelloWorldOptionsApi",
  data() {
    return {
      test: "ma donnée de test",
    };
  },
  methods: {},
  created() {
    const paramValue = this.$route.params.monParam;
    console.log("Received parameter:", paramValue);
  },
};
</script>

<template>
  <div>
    <h1>Hello from Options API Component</h1>
    <p>Data from test property: {{ test }}</p>
  </div>
</template>

<style scoped>

</style>