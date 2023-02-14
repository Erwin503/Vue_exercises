<template>
  <div class="body">
    <div class="main">
      <ul>
        <li v-for="i in obj">{{ i }}</li>
      </ul>
    </div>
    <div class="main">
      <ul>
        <li v-for="(elem, key) in obj">{{ key }} - {{ elem }}</li>
      </ul>
    </div>
    <div class="main">
      <ul>
        <li v-for="(elem, key, num) in obj">
          {{ key }} - {{ elem }} - {{ num }}
        </li>
      </ul>
    </div>
    <div class="main">
      <ul>
        <li v-for="(elem, key, num) in obj">
          {{ key }} - {{ elem }} - {{ num + 1 }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      obj: {
        user1: "100$",
        user2: "200$",
        user3: "300$",
      },
    };
  },
  methods: {
    toggle: function (n) {
      this.visible = !this.visible;
    },
  },
};
</script>
