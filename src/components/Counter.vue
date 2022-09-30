<template>
  <div>
    <h2>Hola como estas {{ person.name }}</h2>
  </div>
</template>

<script>
import { Person } from "@/models/Person";

export default {
  name: "Counter",
  props: {
    person: {
      type: Person,
      required: true,
      validator(value) {
        return value.id !== 0;
      },
    },
  },
};
</script>

<style scoped></style>
