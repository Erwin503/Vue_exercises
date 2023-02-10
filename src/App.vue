<template>
  <div class="body">
    <div class="main">
      <p v-if="isAdmin">Ervin</p>
      <p v-else>Not Ervin</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isAdmin: false,
    };
  },
  // methods: {
  //   toggle: function (n) {
  //     this.visible[n] = !this.visible[n];
  //   },
  // },
};
</script>
