<template>
  <div class="body">
    <div class="main">
      <p>Task 1. Выберите день недели.</p>
      <select v-model="selected">
        <option v-for="option in options">{{ option }}</option>
      </select>
    </div>
    <div class="main">
      <p>Task 2. Выберите день, месяц, год.</p>
      <select v-model="a">
        <option v-for="option in days">{{ option }}</option>
      </select>
      <select v-model="b">
        <option v-for="option in month">{{ option }}</option>
      </select>
      <select v-model="c">
        <option v-for="option in year">{{ option }}</option>
      </select>
    </div>
  </div>
</template>

<script>
let date = new Date();

export default {
  data() {
    return {
      selected: "Понедельник",
      options: [
        "Понедельник",
        "Вторник",
        "Среда",
        "Четверг",
        "Пятница",
        "Суббота",
        "Воскресенье",
      ],
      a: date.getDate(),
      b: date.getMonth(),
      c: date.getFullYear(),
      days: [
        1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20,
        21, 22, 23, 24, 25, 26, 27, 28, 29, 30,
      ],
      month: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
      year: [2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023],
    };
  },

  methods: {},
};
</script>
