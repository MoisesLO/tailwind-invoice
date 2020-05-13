<template>
  <div class="bg-gray-100 h-screen">
    <!-- Menu Header -->
    <nav class="py-8">
      <div class="container mx-auto flex justify-between justify-center">        

        <!-- Logo -->
        <router-link to="/">
          <img class="h-8 w-auto sm:h-10 -mt-2" src="https://plausible.io/assets/images/icon/plausible_logo.compressed.png" alt="Plausible logo">
        </router-link>

        <!-- Menu Medio -->
        <div>
          <router-link to="/" class=" font-medium text-gray-600 hover:text-gray-900">Documentos</router-link>
          <router-link to="/" class="ml-8 font-medium text-gray-600 hover:text-gray-900">Documentos</router-link>
        </div>

        <!-- Menu Derecho -->
        <div>
          <ul class="flex">
            <li>
              <router-link to="/" class=" font-medium text-gray-600 hover:text-gray-900">Login</router-link>
            </li>
            <li class="ml-6">
              <router-link to="/" class=" px-5 py-2 border border-transparent text-base leading-6 font-medium rounded shadow text-white bg-indigo-600 hover:bg-indigo-500 focus:outline-none focus:shadow-outline transitio duration-150 ease-out">Register</router-link>
            </li>
          </ul>
        </div>


      </div>
    </nav>
    <!-- End Menu Header -->

    <div class="pb-12">
      Simple and privacy-friendly alternative to Google Analytics
    </div>
  </div>
</template>