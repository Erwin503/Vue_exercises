<template>
  <div class="main">
    <div id="cmd_head">
      <p>Console</p>
    </div>

    <div id="cmd">
      <p :class="obj">оригинальный текст</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      obj: {
        done: false,
        selected: true,
      },
    };
  },

  methods: {},
};
</script>
