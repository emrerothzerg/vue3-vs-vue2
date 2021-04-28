<template>
  <p>UpperCaseName: {{ upperCaseName }} out of {{ name }}</p>
</template>
<script>
export default {
  data() {
    return {
      name: "Emre",
    };
  },
  computed: {
    upperCaseName() {
      return this.name.toUpperCase();
    },
  },
};
</script>
