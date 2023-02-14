<template>
  <div class="body">
    <div class="main">
      <template v-for="i in items">
        <p v-if="i > 0">{{ i }}</p>
      </template>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return { items: [1, -2, 3, -4, 5] };
  },
  methods: {},
};
</script>
