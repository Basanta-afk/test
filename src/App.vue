<template>
  <div class="container">
    <Header :title="title" @changeTitle="updateTitle($event)" />
    <Content :infos="infos" />
  </div>
</template>

<script>
import Header from "./components/Header";
import Content from "./components/Content";
export default {
  name: "App",
  components: {
    Header,
    Content,
  },
  data() {
    return {
      title: "This is header",
      infos: [
        {
          id: 1,
          name: "Basanta",
          task: "props",
        },
        {
          id: 2,
          name: "Hari",
          task: "props",
        },
        {
          id: 3,
          name: "Shyam",
          task: "props",
        },
        {
          id: 4,
          name: "Gopal",
          task: "props",
        },
        {
          id: 5,
          name: "Aayus",
          task: "props",
        },
      ],
    };
  },
  methods: {
    updateTitle: function (updatedTitle) {
      this.title = updatedTitle;
    },
  },
};
</script>

<style></style>
