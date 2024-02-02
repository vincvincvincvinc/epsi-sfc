<script>
import HelloWorldOptionsApi from "@/components/HelloWorldOptionsApi.vue";
import ChildComponent from "@/components/ChildComponent.vue";

export default {
  components: {
    HelloWorldOptionsApi,
    ChildComponent,
  },
  methods: {
    maMethodePerso() {
      console.log("Event from child component received in parent!");
    },
  },
};
</script>

<template>
<div>
  <HelloWorldOptionsApi msg="Mon message" @monEventPerso="maMethodePerso" />
  <ChildComponent @monEventPerso="maMethodePerso" />
</div>
</template>

<style scoped>

</style>