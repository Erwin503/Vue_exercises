<template>
  <div class="body">
    <div class="main">
      <div id="cmd">
        <p :class="obj">1</p>
        <p class="done">2</p>
      </div>
    </div>
    <div class="main">
      <button @click="hide">Hide</button>
    </div>
    <div class="main">
      <button @click="show">Show</button>
    </div>
    <div class="main">
      <button @click="toggle">Toggle</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      obj: {
        hidden: true,
        done: true,
      },
    };
  },

  methods: {
    hide: function () {
      this.obj.hidden = true;
    },
    show: function () {
      this.obj.hidden = false;
    },
    toggle: function () {
      this.obj.hidden = !this.obj.hidden;
    },
  },
};
</script>
