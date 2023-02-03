<template>
  {{ show() }}
  <div class="body">
    <div class="main"></div>
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
