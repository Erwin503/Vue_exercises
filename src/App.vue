<template>
  <div class="body">
    <div class="main">
    <Emploee :name_person="name" :salary="salary" :age="age" />
    </div>
  </div>
</template>

<script>
import Emploee from "./components/Emploee.vue";

export default {
  data() {
    return {
      name: "John",
      salary: 2000,
      age: 25,
    };
  },
  components: {
    Emploee,
  },
};
</script>
