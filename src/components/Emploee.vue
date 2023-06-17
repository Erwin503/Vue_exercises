<template>
  <div class="body">
    <div class="main">
      <button @click="x">Button number 1</button>
    </div>
    <div class="main">
      <button @click="y">Button number 2</button>
    </div>
  </div>
</template>

<script>
export default {
  emits: ["first", "second"],
  data() {
    return {};
  },
  methods: {
    x() {
      this.$emit("first");
    },
    y() {
      this.$emit("second");
    },
  },
};
</script>
