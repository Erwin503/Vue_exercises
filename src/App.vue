<template>
  <div class="body">
    <div class="main">
      <p>{{ name }}</p>
    </div>
    <div class="main">
      <p>{{ surn }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "Ervin",
      surn: "Smith",
    };
  },
};
</script>
