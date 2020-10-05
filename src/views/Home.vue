<template>
  <div class="home">
    <HelloWorld @show="showMyDiv" />
    <div class="message" v-if="show === true">Hello!</div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  data() {
    return {
      show: false,
    };
  },
  components: {
    HelloWorld,
  },
  methods: {
    showMyDiv() {
      this.show = true;
    },
  },
};
</script>
<style scoped>
.message {
  font-size: 2rem;
}
</style>