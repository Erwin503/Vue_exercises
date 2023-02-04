<template>
  <div class="body">
    <div class="main">
      <a href="fake.html" v-on:click.prevent
        ><p>Tap here and nothing will happen</p></a
      >
    </div>
    <div class="main">
      <button v-on:click.once="haha">haha</button>
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
    haha: function (i) {
      alert("haha");
      return false;
    },
  },
};
</script>
