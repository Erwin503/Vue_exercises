<template>
  <div class="body">
    <div class="main">
      <button @click="show()">On click</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      num1: 1,
      num2: 2,
    };
  },
  methods: {
    show: function () {
      alert(this.num1 + this.num2);
    },
  },
};
</script>
