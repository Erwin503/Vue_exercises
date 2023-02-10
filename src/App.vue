<template>
  <div class="body">
    <div class="main">
      <p v-if="visible[0]">Ervin</p>
      <button @click="toggle(0)">{{ visible[0] ? "hide" : "show" }}</button>
    </div>
    <div class="main">
      <p v-if="visible[1]">Ervin</p>
      <button @click="toggle(1)">{{ visible[1] ? "hide" : "show" }}</button>
    </div>
    <div class="main">
      <p v-if="visible[2]">Ervin</p>
      <button @click="toggle(2)">{{ visible[2] ? "hide" : "show" }}</button>
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
