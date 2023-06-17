<template>
  <div class="body">
    <div class="main">
      <p>В каком городе вы живете.</p>
      <select v-model="selected">
        <option>Симферополь</option>
        <option>Москва</option>
        <option>Питер</option>
      </select>

      <p>{{ selected }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selected: "",
    };
  },

  methods: {},
};
</script>
