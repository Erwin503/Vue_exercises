<template>
  <div class="body">
    <div class="main">
      <button @click="show(2)">2</button>
    </div>
    <div class="main">
      <button @click="show(3)">3</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {},
  methods: {
    show: function (i) {
      alert(i ** 2);
    },
  },
};
</script>
