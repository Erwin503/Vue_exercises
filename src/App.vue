<template>
  <div class="body">
    <div class="main">
      <ul>
        <li v-for="p in products" :key="p.id">{{ p.name }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1,
          name: "product1",
        },
        {
          id: 2,
          name: "product2",
        },
        {
          id: 3,
          name: "product3",
        },
      ],
    };
  },
  methods: {},
};
</script>
