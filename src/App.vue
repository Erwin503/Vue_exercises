<template>
  <div class="body">
    <div class="main">
      <ul>
        <li v-for="i in hrefs">
          <a href="{{ i.href }}">{{ i.text }}</a>
        </li>
      </ul>
    </div>
    <div class="main">
      <tr v-for="p in products">
        <td>{{ p.name }}</td>
        <td>{{ p.price }}</td>
        <td>{{ p.quantity }}</td>
      </tr>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      hrefs: [
        { href: "1.html", text: "text1" },
        { href: "2.html", text: "text2" },
        { href: "3.html", text: "text3" },
      ],
      products: [
        {
          name: "product1",
          price: 100,
          quantity: 5,
        },
        {
          name: "product2",
          price: 200,
          quantity: 4,
        },
        {
          name: "product3",
          price: 300,
          quantity: 3,
        },
      ],
    };
  },
  methods: {
    toggle: function (n) {
      this.visible = !this.visible;
    },
  },
};
</script>
