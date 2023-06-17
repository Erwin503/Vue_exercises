<template>
  <div class="body">
    <div class="main">
      <p>Введите текст</p>
      <input v-model="newItem" />
    </div>
    <div class="main">
      <button @click="addItem">Press me!</button>
      <ul>
        <li v-for="(item, index) in arr" :key="index">
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
let date = new Date();

export default {
  data() {
    return {
      newItem: "",
      arr: ["lala", "haha"],
    };
  },

  methods: {
    addItem: function () {
      this.arr.unshift(this.newItem);
    },
  },
};
</script>
