<template>
  <div>Name: {{ name }}</div>
</template>
<script>
import { ref } from "vue";
export default {
  setup() {
    const name = ref('Emre');
    return { name };
  }
};
</script>