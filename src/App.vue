<template>
  <div class="body">
    <div class="main">
      <p>Task 1</p>
      <input type="checkbox" v-model="arr" value="Python" /> <span>Python</span
      ><br />
      <input type="checkbox" v-model="arr" value="Java" /> <span>Java</span
      ><br />
      <input type="checkbox" v-model="arr" value="JS" /> <span>JS</span><br />
    </div>
    <div class="main">
      <input type="checkbox" v-model="arr" value="C++" /> <span>C++</span><br />
      <input type="checkbox" v-model="arr" value="C" /> <span>C</span><br />
      <input type="checkbox" v-model="arr" value="GO" /> <span>GO</span><br />
      <input type="checkbox" v-model="arr" value="Ruby" /> <span>Ruby</span
      ><br />
    </div>

    <div class="main">
      <p>Количество: {{ arr.length }}</p>
      <p>Cписок языков:</p>
      <ul v-for="elem in arr">
        <li>{{ elem }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arr: [],
    };
  },

  methods: {},
};
</script>
