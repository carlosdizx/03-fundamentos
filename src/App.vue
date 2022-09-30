<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Counter :person="person" />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Counter from "@/components/Counter.vue";
import { Person } from "@/models/Person";

export default defineComponent({
  name: "App",
  components: { Counter },
  data: () => ({
    person: new Person(0, "Ernesto"),
  }),
});
</script>

<style></style>
