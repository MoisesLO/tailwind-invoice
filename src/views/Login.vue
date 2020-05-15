<template>
  <div class=" bg-gray-100 min-h-screen">    
    
    <div class="mx-auto w-full max-w-md h-full pt-24 ">

      <h1 class="text-center text-2xl text-gray-600 pb-5">Lineysoft <span class=" text-xs">.com</span></h1>

      <form class="shadow-md rounded px-8 py-6 mb-4 bg-white">
        <p class=" text-base text-gray-600">Coloca tu Usuario y contrasena</p>
        <div class="mb-6 mt-6">
          <label class="block text-gray-600 text-sm font-bold mb-2" for="username">Usuario:</label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            v-model="user.email"
            id="username"
            type="text"
            placeholder="Username"
          />
        </div>
        <div class="mb-6">
          <label class="block text-gray-600 text-sm font-bold mb-2" for="password">Contrasenia:</label>
          <input
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline"
            v-model="user.password"
            id="password"
            type="password"
            placeholder="******************"
          />
          <!--<p class="text-red-500 text-xs italic">Please choose a password.</p>-->
        </div>
        <div class="">
          <button
            class="bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-2 px-4 
            rounded focus:outline-none focus:shadow-outline w-full"
            type="button">Entrar →</button>
          <div class=" pt-5 text-center text-xs text-gray-500">
            No tienes una cuenta ? Registrate ahora.
          </div>
          
        </div>
      </form>
      <p class="text-center text-gray-500 text-xs">&copy;2020 Acme Corp. All rights reserved.</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        email: "demo@gmail.com",
        password: "demo1234556"
      }
    };
  }
};
</script>