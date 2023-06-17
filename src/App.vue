<template>
  <div class="body">
    <div class="main">
      <p>Task 1</p>
      <input v-bind:disabled="isDisabled" />
      <br />
      <input type="checkbox" v-model="isDisabled" />
      <span>Заблокировать input</span>
    </div>
  </div>
</template>

<script>
let date = new Date();

export default {
  data() {
    return {
      isDisabled: true,
    };
  },

  methods: {
    block: function () {
      this.isDisabled = !this.isDisabled;
    },
  },
};
</script>
