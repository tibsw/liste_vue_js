<template>
  <h1>Hello world</h1>
  <ul id="tableau">
    <li v-show="toggle" v-for="item in items" :key="item.name">
      
      {{ item.name }}
    </li>
  </ul>
  <button @click="toggle = !toggle">Afficher/Cacher</button>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data: function () {

    return {
toggle: true,
      items: [

        { name: "Melvyn REBECA" },
        { name: "Thibault SOWA" },
        { name: "Melvyn REBECA" },
        { name: "Thibault SOWA" },
        { name: "Melvyn REBECA" },
        { name: "Thibault SOWA" },
        { name: "Melvyn REBECA" },

      ],

    };

  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
