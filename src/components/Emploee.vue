<script>
export default {
  emits: ["show", "show1"],
  data() {
    return {};
  },
  methods: {
    aaa() {
      this.$emit("show");
    },
    bbb() {
      this.$emit("show1");
    },
  },
};
</script>

<template>
  <div class="body">
    <div class="main">
      <button @click="aaa">BMW</button>
    </div>
    <div class="main">
      <button @click="bbb">bmw</button>
    </div>
  </div>
</template>
