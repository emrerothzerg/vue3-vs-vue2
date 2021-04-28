<template>
  <div>
    <input type="text" v-model="name" />
    <div>Name: {{ name }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
    };
  },
  watch: {
    name(newVal, oldVal) {
      console.log(`${newVal} ${oldVal}`);
    },
  },
};
</script>
