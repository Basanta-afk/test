<template>
  <header>
    <h1>{{ title }}</h1>
    <button @click="changeTitle">Update</button>
    <!-- <Button text="change" color="green" /> -->
  </header>
</template>

<script>
// import Button from "./Button";

export default {
  name: "Header",
  props: {
    title: String,
  },
  methods: {
    changeTitle: function () {
      this.$emit("changeTitle", "hi");
    },
  },
  //   components: {
  //     Button,
  //   },
};
</script>

<style></style>
