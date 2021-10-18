<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <h1>{{ title }}</h1>
    <label for="">Name</label><br />
    <input type="text" v-model="name" />

    <br /><br />
    <label for="">Fone</label><br />
    <input type="text" v-model="fone" />

    <br /><br />
    <label for="">you wish recerve News</label><br />
    <input type="radio" v-model="news" /> yes
    <input type="radio" v-model="news" /> No

    <br /><br />
    <label for="">intersting</label><br />
    <input type="checkbox" v-model="intersting" /> moda
    <input type="checkbox" v-model="intersting" /> sport
    <input type="checkbox" v-model="intersting" /> beauty

    <br /><br />
    <label for="">how you met us</label><br />
    <select v-model="met">
      <option value="">choice</option>
      <option value="Google">Google </option
      ><option value="social media">choice </option></select
    >
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  data: () => {
    return {
      titulo: "doing forms",
      firstName: "",
      lastName: "",
    };
  },
  computed: {},
  methods: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
