<template>
    <Emploee @func="func" />
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
    func(name, salary) {
      console.log(name, salary);
    },
  },
};
</script>
