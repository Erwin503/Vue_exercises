<template>
  <div class="body">
    <div class="main">
      <p>Нажмите на элемент списка для удаления</p>
      <ul>
        <li
          v-for="(item, index) in arr"
          :key="index"
          @click="removeItem(index)"
        >
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
let date = new Date();

export default {
  data() {
    return {
      arr: ["1", "2", "3", "4", "5"],
    };
  },

  methods: {
    removeItem: function (index) {
      this.arr.splice(index, 1);
    },
  },
};
</script>
