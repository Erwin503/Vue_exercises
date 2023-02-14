<template>
  <div class="body">
    <div class="main">
      <div v-if="visible">
        <p>ERVIN</p>
        <p>ERVIN</p>
        <p>ERVIN</p>
      </div>
    </div>
    <dib class="main">
      <button @click="toggle">Toggle</button>
    </dib>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible: true,
    };
  },
  methods: {
    toggle: function (n) {
      this.visible = !this.visible;
    },
  },
};
</script>
