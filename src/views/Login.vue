<template>
  <div class="mx-auto w-full max-w-xs h-full my-24">
    <h1 class="text-center text-2xl text-gray-700">Login</h1>

    <form class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4">
      <div class="mb-4">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="username">
          Usuario
        </label>
        <input
            class="shadow appearance-none
            border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            v-model="user.email"
            id="username" type="text" placeholder="Username">
      </div>
      <div class="mb-6">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="password">
          Contrasenia
        </label>
        <input
            class="shadow appearance-none border rounded w-full py-2 px-3
            ext-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline"
            v-model="user.password"
            id="password" type="password" placeholder="******************">
        <!--<p class="text-red-500 text-xs italic">Please choose a password.</p>-->
      </div>
      <div class="flex items-center justify-between">
        <button
            class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
            type="button">
          Entrar
        </button>
        <a class="inline-block align-baseline font-bold text-sm text-blue-500 hover:text-blue-800" href="#">
          Recordar Contrasena?
        </a>
      </div>
    </form>
    <p class="text-center text-gray-500 text-xs">
      &copy;2020 Acme Corp. All rights reserved.
    </p>
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
      }
    }

  }
</script>