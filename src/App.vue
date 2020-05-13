<template>
  <div id="app">    
    <Navbar v-if="layout=='admin'"></Navbar>

    <!-- Mega Menu -->
    <!--<div class="relative">
        <a href class>Megamenu</a>
        <div
          class="absolute normal-case font-normal bg-white shadow-md rounded-lg overflow-hidden border mt-4" style=" left: -60px"
        >
          <div class="flex px-8 py-6 border-b -mx-4">
            <div class="w-1/2 px-4">
              lorem ipsum
            </div>
            <div class="w-1/2 px-4">
              lorem ipsum
            </div>
          </div>
          <ul class=" bg-gray-100 px-8 py-8">
            <li>Lorem Ipsum</li>
            <li>Lorem Ipsum</li>
            <li>Lorem Ipsum</li>
            <li>Lorem Ipsum</li>
          </ul>

        </div>
    </div>-->
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
      if(this.$router.currentRoute.path == '/' || this.$router.currentRoute.path == '/curve' || this.$router.currentoute.path == '/home'){
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
