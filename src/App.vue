<template>
  <div id="app">    
    <Navbar v-if="layout=='admin'"></Navbar>
    <router-view />
  </div>
</template>

<script>
import Navbar from "../src/components/Navbar";
export default {
  data() {
    return {
      layout: ''
    }
  },
  methods: {
    GetCurrentRoute(){
      if(this.$router.currentRoute.path == '/' || this.$router.currentRoute.path == '/curve' || this.$router.currentRoute.path == '/home'){
        this.layout = '';
      }else{
        this.layout = 'admin';
      }
      console.log(this.$router.currentRoute.path);
    }
  },
  components: {
    Navbar
  },
  watch: {
    '$route'(value) {
      if(value.path == '/' || value.path == '/curve' || value.path == '/home'){
        this.layout = '';        
      }else{
        this.layout = 'admin';
      }      
      console.log(value.path);
    }
  },
  mounted(){
    this.GetCurrentRoute();
  }  
};
</script>

<style lang="scss">
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>
