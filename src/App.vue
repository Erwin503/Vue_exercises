<template>
  <div class="body">
    <div class="main">
      <p>Task 59</p>
      <Emploee name="John" surn="Smit" age="25" />
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
