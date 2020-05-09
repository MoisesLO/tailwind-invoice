<template>
  <div id="app">
    <Navbar></Navbar>
    <div class="container mx-auto">
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
  </div>
</template>

<script>
  import Navbar from '../src/components/Navbar'
  export default {
    data(){
      return{

      }
    },
    components:{
      Navbar
    }

  }
</script>

<style lang="scss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
