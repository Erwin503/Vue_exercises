<template>
  <div class="body">
    <div class="main">
      <p>{{ obj.x + obj.y + obj.z }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      obj: { x: 1, y: 2, z: 3 },
    };
  },
};
</script>
