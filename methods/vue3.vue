<template>
  <div>Count: {{ count }}</div>
  <button @click="increaseCount()">Increase Count</button>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const count = ref(3);
    const increaseCount = () => {
      count.value += 1;
    };
    return { count, increaseCount };
  },
};
</script>
