<template>
  <div class="body">
    <div class="main">
      <ul>
        <li v-for="i in arr">{{ i }}</li>
      </ul>
    </div>
    <div class="main"><button @click="add">add</button></div>
    <div class="main"><button @click="del">del</button></div>
    <div class="main"><button @click="strdel">strdel</button></div>
    <div class="main"><button @click="sort">sort</button></div>
    <div class="main"><button @click="rev">rev</button></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: ["b", "a", "c"],
    };
  },
  methods: {
    add: function () {
      this.arr.push("xxx");
    },
    del: function () {
      this.arr.pop();
    },
    strdel: function () {
      this.arr.splice(this.arr.length - 2, 1);
    },
    sort: function () {
      this.arr.sort();
    },
    rev: function () {
      this.arr.reverse();
    },
  },
};
</script>
