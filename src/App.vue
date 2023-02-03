<template>
  <div class="body">
    <div class="main">
      <button @click="show()">On click</button>
    </div>
    <div class="main">
      <button v-on:mouseover="show()">Come here</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {},
  methods: {
    show: function () {
      var date = new Date();
      alert(date);
    },
  },
};
</script>
