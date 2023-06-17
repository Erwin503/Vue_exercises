<template>
  <div class="body">
    <div class="main">
      <p>Task 1</p>
      <input type="checkbox" v-model="checked" />
      <p v-if="checked">Test</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      checked: false,
    };
  },

  methods: {
    press: function () {
      this.checked = !this.checked;
    },
  },
};
</script>
