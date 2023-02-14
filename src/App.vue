<template>
  <div class="body">
    <div class="main">
      <div v-for="i in items">{{ i }}</div>
    </div>
    <div class="main">
      <div v-for="i in items">{{ i ** 2 }}</div>
    </div>
    <div class="main">
      <ul>
        <li v-for="i in items">{{ i }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [1, 2, 3, 4, 5],
    };
  },
  methods: {
    toggle: function (n) {
      this.visible = !this.visible;
    },
  },
};
</script>
