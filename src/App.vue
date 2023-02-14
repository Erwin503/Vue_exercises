<template>
  <div class="body">
    <div class="main">
      <div v-for="i in items">
        <p>{{ i }}</p>
        <p class="divider"></p>
      </div>
    </div>
    <div class="main">
      <ul>
        <template v-for="i in items">
          <li>{{ i }}</li>
          <li class="divider"></li>
        </template>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [1, 2, 3],
    };
  },
  methods: {
    toggle: function (n) {
      this.visible = !this.visible;
    },
  },
};
</script>
