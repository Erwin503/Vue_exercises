<template>
  <div class="body">
    <div class="main">
      <ul>
        <li v-for="(i, key) in arr">{{ key }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: ["x", "y", "z"],
    };
  },
  methods: {
    toggle: function (n) {
      this.visible = !this.visible;
    },
  },
};
</script>
