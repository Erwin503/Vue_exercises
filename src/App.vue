<template>
  <div class="body">
    <div class="main">
      <p>Task 1</p>
      <textarea v-model="text"></textarea>
      <p>{{ text }}</p>
    </div>
    <div class="main">
      <p>Task 2</p>
      <textarea v-model="txt"></textarea>
      <button @click="press">Calculate</button>
      <ul v-for="elem in arr">
        <li>{{ elem }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: 0,
      txt: 0,
      arr: [],
    };
  },

  methods: {
    press: function () {
      this.arr = this.txt.split(" ");
    },
  },
};
</script>
