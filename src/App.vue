<template>
  <div class="body">
    <div class="main">
      <button @click="calc">Task 1</button>
    </div>
    <div class="main">
      <button @click="sum">Task 2</button>
    </div>
    <div class="main">
      <button @click="transpos">Task 3</button>
    </div>
    <div class="main">
      <button @click="fiosep">Task 4</button>
    </div>
  </div>

  <div class="body">
    <div class="main">
      <p> Task 1</p>
      <p> Введите число</p>
      <input v-model="num" />
      <p>--- Результат ---</p>
      <p> {{ res }}</p>
      <br />
    </div>
    <div class="main">
      <p> Task 2</p>
      <p> Введите числа</p>
      <input v-model="num1" />
      <input v-model="num2" />
      <p>--- Результат ---</p>
      <p> {{ res_2 }}</p>
      <br />
    </div>
    <div class="main">
      <p> Task 3</p>
      <p> Введите строки</p>
      <input v-model="str1" />
      <input v-model="str2" />
      <p>--- Результат ---</p>
      <p> {{ str1 }}</p>
      <p> {{ str2 }}</p>
      <br />
    </div>
    <div class="main">
      <p> Task 4</p>
      <p> Введите ФИО:</p>
      <input v-model="fio" />
      <p>--- Результат ---</p>
      <p> Имя: {{ name }}</p>
      <p> Фамилия: {{ surname }}</p>
      <p> Отчество: {{ namefat }}</p>
    </div>
  </div>
  <div id="cmd"></div>
</template>

<script>
export default {
  data() {
    return {
      num: 0,
      res: 0,

      num1: "",
      num2: 0,
      res_2: 0,

      str1: "",
      str2: "",
      buf: "",

      fio: "",
      name: "",
      surname: "",
      namefat: "",
    };
  },

  methods: {
    calc: function () {
      this.res = this.num ** 2;
    },
    sum: function () {
      this.res_2 = Number(this.num1) + Number(this.num2);
    },
    transpos: function () {
      this.buf = this.str1;
      this.str1 = this.str2;
      this.str2 = this.buf;
    },
    fiosep: function () {
      let arr = this.fio.split(" ");
      (this.name = arr[0]), (this.surname = arr[1]), (this.namefat = arr[2]);
    },
  },
};
</script>
