<template>
  <p>UpperCaseName: {{ upperCaseName }} out of {{ name }}</p>
</template>
<script>
import { ref, computed } from "vue";
export default {
  setup() {
    const name = ref("Emre");
    const upperCaseName = computed(() => {
      return name.value.toUpperCase();
    });
    return { name, upperCaseName };
  },
};
</script>
