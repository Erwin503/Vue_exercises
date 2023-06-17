<template>
  <div class="body">
    <div class="main">
      <p :style="{ color: 'rgb(4, 194, 118)', 'background-color': 'yellow' }">
        Зеленый шрифт с желтым фоном.
      </p>
      <p :style="{ 'font-style': 'italic', 'font-weight': 'bold' }">
        Абзац жирный и курсивный.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },

  methods: {},
};
</script>
