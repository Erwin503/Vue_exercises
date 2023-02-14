<template>
  <div class="body">
    <div class="main">
      <p v-if="age < 18">Подросток</p>
      <p v-else-if="age > 18 && age < 26">молодой человек</p>
      <p v-else-if="age > 25">мужчина</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      age: 25,
    };
  },
  // methods: {
  //   toggle: function (n) {
  //     this.visible[n] = !this.visible[n];
  //   },
  // },
};
</script>
