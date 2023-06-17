<template>
  <div id="cmd">
    <Emploee @first="one" @second="two" />
  </div>
</template>

<script>
import Emploee from "./components/Emploee.vue";

export default {
  data() {
    return {};
  },
  components: {
    Emploee,
  },
  methods: {
    one() {
      alert("Первая функция");
    },
    two() {
      alert("Вторая функция");
    },
  },
};
</script>
