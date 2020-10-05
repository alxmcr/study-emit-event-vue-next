<template>
  <div class="btn" @click="showDiv">CLICK me!!</div>
</template>

<script>
export default {
  name: "HelloWorld",
  methods: {
    showDiv() {
      this.$emit("show", true);
    },
  },
};
</script>
<style scoped>
.btn {
  border-radius: 15px;
  border: 1px solid black;
}
</style>