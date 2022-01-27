<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Go Go" color="green" />
  </header>
</template>

<script>
import Button from "./Button";

export default {
  name: "Header",
  props: {
    title: String,
  },
  components: {
    Button,
  },
};
</script>

<style></style>
