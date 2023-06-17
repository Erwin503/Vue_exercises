<template>
  <div class="body">
    <div class="main">
      <p>Task 60</p>
      <Emploee :arr="['Ervin', 'Smith', 25]" />
    </div>
  </div>
</template>

<script>
import Emploee from "./components/Emploee.vue";

export default {
  components: {
    Emploee,
  },
};
</script>
