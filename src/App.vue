<template>
  <div class="body">
    <div class="main">
      <p v-if="visible[0]">Ervin</p>
      <button @click="toggle(0)">toggle</button>
    </div>
    <div class="main">
      <p v-if="visible[1]">Ervin</p>
      <button @click="toggle(1)">toggle</button>
    </div>
    <div class="main">
      <p v-if="visible[2]">Ervin</p>
      <button @click="toggle(2)">toggle</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible: [true, true, true],
    };
  },
  methods: {
    toggle: function (n) {
      this.visible[n] = !this.visible[n];
    },
  },
};
</script>
