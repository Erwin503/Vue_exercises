<template>
  <div class="body">
    <div class="main">
      <p :class="{ active: isDisabled, valid: isValid }">Test</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isValid: true,
      isDisabled: true,
    };
  },

  methods: {},
};
</script>
