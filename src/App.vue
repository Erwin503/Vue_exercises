<template>
  <div class="body">
    <div class="main">
      <p v-if="visible">Ervin</p>
    </div>
    <div class="main">
      <button @click="hide" v-if="visible">hide</button>
    </div>
    <div class="main">
      <button @click="show" v-if="!visible">show</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible: false,
    };
  },
  methods: {
    hide: function () {
      this.visible = false;
    },
    show: function () {
      this.visible = true;
    },
  },
};
</script>
