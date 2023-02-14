<template>
  <div class="body">
    <div class="main">
      <div v-show="visible">
        <p>ERVIN</p>
        <p>ERVIN</p>
        <p>ERVIN</p>
        <!-- 2 задание
        v-show отрисовывается всегда и меняется только css
        v-if не отрисовывается если значение ложно
        3 задание
        v-show, если переключения будут частыми, и v-if, если условие может и не измениться во время исполнения 
        4 задание
        нельзя использовать v-else-->
      </div>
    </div>
    <dib class="main">
      <button @click="toggle">Toggle</button>
    </dib>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible: true,
    };
  },
  methods: {
    toggle: function (n) {
      this.visible = !this.visible;
    },
  },
};
</script>
