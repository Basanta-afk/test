<template>
  <div>
    <ul>
      <li v-for="info in infos" :key="info.id">
        <h2>
          {{ info.name }}
        </h2>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Content",
  props: {
    infos: Array,
  },
};
</script>

<style></style>
