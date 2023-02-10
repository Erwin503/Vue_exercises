<template>
  <div class="body">
    <div class="main">
      <p v-if="day === 1">Monday</p>
      <p v-if="day === 2">Tuesday</p>
      <p v-if="day === 3">Wednesday</p>
      <p v-if="day === 4">Thursday</p>
      <p v-if="day === 5">Friday</p>
      <p v-if="day === 6">Saturday</p>
      <p v-if="day === 7">Sunday</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      day: 4,
    };
  },
  // methods: {
  //   toggle: function (n) {
  //     this.visible[n] = !this.visible[n];
  //   },
  // },
};
</script>
