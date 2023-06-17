<template>
  <div class="body">
    <div class="main">
      <p>Введите текст</p>
      <input v-on:keypress.enter="submit" v-model="txt" />
      <p>{{ task1 }}</p>
    </div>
    <div class="main">
      <p>Нажмите на ссылку</p>
      <a @click.a="link">Press me + a</a>
      <p> {{ task2 }}</p>
    </div>
    <div class="main">
      <p>Нажмите на ссылку</p>
      <a @click.left="link1" @click.right="link2" @click.middle="link3"
        >Press me</a
      >
      <p> {{ task3 }}</p>
    </div>
  </div>
</template>

<script>
let date = new Date();

export default {
  data() {
    return {
      task1: "",
      txt: "",

      task2: "",
      task3: "",
    };
  },

  methods: {
    submit: function () {
      this.task1 = this.txt;
    },
    link: function () {
      this.task2 = "Вы нажали на ссылку с зажатой клавишей a.";
    },
    link1: function () {
      this.task3 = "left";
    },
    link2: function () {
      this.task3 = "right";
    },
    link3: function () {
      this.task3 = "middle";
    },
  },
};
</script>
