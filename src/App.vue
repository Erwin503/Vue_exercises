<template>
  <div class="body">
    <div class="main">
      <p>{{ num ** 2 }}</p>
    </div>
    <div class="main">
      <p>{{ num1 + num2 + num3 }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      num: 5,
      num1: 1,
      num2: 2,
      num3: 3,
    };
  },
};
</script>
