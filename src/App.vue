<template>

  <div class="main">
    <div id="cmd_head">
      <p>Console</p>
    </div>
    <div id="cmd">
      <p :class="cssClasses">Тест</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cssClasses: "test",
    };
  },

  methods: {},
};
</script>
