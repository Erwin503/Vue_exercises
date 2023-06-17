<template>

  <div id="cmd">
    <Emploee
      v-for="user in users"
      :name="user.name"
      :salary="user.salary"
      :id="user.id"
      :age="user.age"
      :key="user.id"
    />
  </div>
</template>

<script>
import Emploee from "./components/Emploee.vue";

export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: "name1",
          salary: 100,
          age: 30,
        },
        {
          id: 2,
          name: "name2",
          salary: 200,
          age: 40,
        },
        {
          id: 3,
          name: "name3",
          salary: 300,
          age: 50,
        },
      ],
    };
  },
  components: {
    Emploee,
  },
};
</script>
