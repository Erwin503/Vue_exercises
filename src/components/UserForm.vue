<template>
  <div class="body">
    <div class="main">
      <input v-model="newName" />
      <input v-model="newSurn" />

      <button @click="save">save</button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      newName: "",
      newSurn: "",
    };
  },
  methods: {
    save() {
      this.$emit("add", this.newName, this.newSurn);
      this.newName = "";
      this.newSurn = "";
    },
  },
};
</script>
