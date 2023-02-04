<template>
  <div class="body">
    <div class="main">
      <p>{{ cost }}</p>
      <p>{{ amount }}</p>
      <p>{{ price }}</p>
    </div>
    <div class="main">
      <button @click="change(text)">+</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cost: 10,
      amount: 2,
    };
  },
  methods: {
    change: function (i) {
      this.cost = this.cost + 1;
    },
  },
  computed: {
    price: function () {
      return this.cost * this.amount;
    },
  },
};
</script>
