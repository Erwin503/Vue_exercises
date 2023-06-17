<template>
  <div class="body">
    <div class="main">
      {{ name }}
      {{ surn }}
    </div>
    <div class="main">
      <button @click="$emit('remove', id)">remove</button>
      <br />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    id: Number,
    name: String,
    surn: String,
  },
  emits: ["remove"],
  data() {
    return {};
  },
  methods: {},
};
</script>
