<script>
import Navbar from './components/Navbar.vue'
export default {
  name: "app",
  components: {
    Navbar,
  },
  data(){
    return {
      
    }
  },
  methods: {
  },
  computed:{
  },
  created(){
    // call initState() from store
  }
}
</script>

<template>
  <Navbar />
  <div class="content-container">
    <router-view />
  </div>
</template>

<style>
@import "@/assets/base.css";

body {
  margin: 0;
  padding: 0;
  background-color: #222;
  height: 100%;
}

a:link, a:visited, a:hover, a:active {
  color: transparent;
}

#app{
  display: flex;
  flex-flow: column;
  height: 100vh;
}

.content-container {
  height: 100%;
  display: flex;
  align-content: center;
  justify-content: center;
  /* height: 100%;
  width: 100vw; */
  min-width: 600px;
  min-height: 400px;
  box-sizing: border-box;
  /* border: green 10px solid; */
}

* {  
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  box-sizing: border-box;         /* Opera/IE 8+ */
}
</style>