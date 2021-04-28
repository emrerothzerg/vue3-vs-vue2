<template>
  <div>{{ formatUnix(new Date()) }}</div>
</template>

<script>
import formatUnix from "./filter.js";
export default {
  name: "App",
  setup() {
    return {
      formatUnix,
    };
  },
};
</script>
