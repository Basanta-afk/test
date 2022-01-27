<template>
  <div class="container">
    <Header title="This is Header" />
    <Content :infos="infos" />
    <Footer title="This is Footer" />
  </div>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer";
import Content from "./components/Content";
export default {
  name: "App",
  components: {
    Header,
    Footer,
    Content,
  },
  data() {
    return {
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
};
</script>

<style></style>
