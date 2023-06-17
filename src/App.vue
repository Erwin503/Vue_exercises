<template>
  <div class="body">
    <div class="main">
      <p>Выберете родной язык.</p>
      <input name="radio" type="radio" v-model="choice" value="rus" />
      <span> Русский</span><br />

      <input name="radio" type="radio" v-model="choice" value="tat" />
      <span> Крымскотатарский</span><br />

      <input name="radio" type="radio" v-model="choice" value="eng" />
      <span> Английский</span><br />
    </div>
    <div class="main">
      <p v-if="choice == 'rus'">Русский язык</p>
      <p v-if="choice == 'tat'">Къырымтатар тили</p>
      <p v-if="choice == 'eng'">English language</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      choice: "",
    };
  },

  methods: {},
};
</script>
