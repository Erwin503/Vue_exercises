<template>
  <div class="body">
    <div class="main">
      <a :href="page">Tap here)</a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      page: "page.html",
    };
  },
};
</script>
