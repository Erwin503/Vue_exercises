<template>
  <div class="body">
    <div class="main">
      <p v-if="visible">Ervin</p>
    </div>
    <div class="main">
      <p v-if="!visible">Ervin</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible: true,
    };
  },
};
</script>
