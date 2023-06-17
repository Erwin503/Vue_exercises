<template>
  <div class="body">
    <div class="main">
      <button @click="$emit('func', 'Ervin', '3000$')">1</button>
    </div>
  </div>
</template>

<script>
export default {
  emits: ["func"],
  data() {
    return {};
  },
  methods: {},
};
</script>
