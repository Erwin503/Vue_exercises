<template>
  <div class="body">
    <div class="main">
      <p>{{ text }}</p>
    </div>
    <div class="main">
      <button @click="change(text)">+</button>
    </div>
    <div class="main">
      <button @click="achange(text)">-</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "Ervin",
    };
  },
  methods: {
    change: function (i) {
      this.text = this.text + " " + "Ervin";
    },
    achange: function (i) {
      this.text = "Ervin";
    },
  },
};
</script>
