<template>
  <BMW @show="BMW" @show1="bmw" />
</template>

<script>
import BMW from "./components/Emploee.vue";
export default {
  data() {
    return {};
  },
  components: {
    BMW,
  },
  methods: {
    BMW() {
      alert("Alex, Jason, Paul");
    },
    bmw() {
      alert("Jace, Tom, Ben");
    },
  },
};
</script>
