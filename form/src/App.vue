<template>
  <div id="app" class="bg-black-300" >
    <HelloWorld msg="Welcome to Form"/>
    <h1>{{ title }}</h1>
    <label>Name</label><br />
    <input type="text" v-model="name" />

    <br /><br />
    <label>Fone</label><br />
    <input type="text" v-model="fone" />

    <br /><br />
    <label>You wish recerving News</label><br />
    <input type="radio" value="yes" v-model="news" /> yes
    <input type="radio" value="No" v-model="news" /> No

    <br /><br />
    <label>Interest</label><br />
    <input type="checkbox" value="moda" v-model="interest" /> moda
    <input type="checkbox" value="sport" v-model="interest" /> sport
    <input type="checkbox" value="beauty" v-model="interest" /> beauty

    <br /><br />
    <label for="">how you met us</label><br />
    <select v-model="met">
      <option value="">choice</option>
      <option value="Google">Google </option
      ><option value="social media">social media</option></select
    >
    <br><br>

    <button>Send</button>

    <hr>
    
    Name: {{ name }} <br>
    Fone: {{ fone }} <br>
    News: {{ news }} <br>
    Intersting: {{ interest }} <br>
    Met: {{ met }} <br>
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
      name: "",
      fone: "",
      news:"",
      interest: [],
      met:"",
    };
  },
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
  background-color:thistle;
}
</style>


