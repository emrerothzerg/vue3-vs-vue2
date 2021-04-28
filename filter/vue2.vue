<template>
  <div>
    {{ new Date() | formatUnix }}
  </div>
</template>

<script>
import moment from "moment";
export default {
  name: "App",
  filters: {
    formatUnix(value) {
      if (value) {
        return moment(value).format("DD/MM/YYYY");
      }
    },
  },
};
</script>
