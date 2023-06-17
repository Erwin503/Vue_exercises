<template>
  <div class="body">
    <div class="main">
      <p>> Введите текст</p>
      <input v-model="task2" />
      <p>{{ task2 }}</p>
    </div>
    <div class="main">
      <p>> Введите число</p>
      <input v-model="task3" />
      <p>> {{ task3 * task3 }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      task3: "hello",
      task2: "qwert",
    };
  },

  methods: {},
};
</script>
