<template>
  <input type="text" v-model="name" />
  <div>Name: {{ name }}</div>
</template>

<script>
import { ref, watch } from "vue";
export default {
  setup() {
    const name = ref("");
    watch(name, (newVal, oldVal) => {
      console.log(`${newVal} ${oldVal}`);
    });
    return { name };
  },
};
</script>
