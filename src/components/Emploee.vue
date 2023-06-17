<template>
  <p>Работник номер {{ id }}</p>
  <p>Name: {{ name }}</p>
  <p>Salary: {{ salary }}$</p>
  <p>Age: {{ age }}</p>
  <br />
</template>

<script>
export default {
  props: {
    id: Number,
    name: String,
    salary: Number,
    age: Number,
  },
  data() {
    return {};
  },
};
</script>
