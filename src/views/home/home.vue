<template>
  <div>
    <!-- Menu Header -->
    <nav class="py-8">
      <div class="mx-auto flex justify-between justify-center  max-w-screen-lg">

        <!-- Logo -->
        <router-link to="/" class=" text-2xl text-gray-700">
          Lineysoft <span class=" text-sm">.com</span>
          <!-- <img class="h-8 w-auto sm:h-10 -mt-2" src="https://plausible.io/assets/images/icon/plausible_logo.compressed.png" alt="Plausible logo"> -->
        </router-link>

        <!-- Menu Medio -->
        <div>
          <router-link to="/" class=" font-medium text-gray-600 hover:text-gray-900">Documentacion</router-link>
          <router-link to="/" class="ml-8 font-medium text-gray-600 hover:text-gray-900">Precios</router-link>
          <router-link to="/" class="ml-8 font-medium text-gray-600 hover:text-gray-900">Blog</router-link>
          <router-link to="/" class="ml-8 font-medium text-gray-600 hover:text-gray-900">Contacto</router-link>
        </div>

        <!-- Menu Derecho -->
        <div>
          <ul class="flex">
            <li>
              <router-link to="/login" class=" font-medium text-gray-600 hover:text-gray-900">Login</router-link>
            </li>
            <li class="ml-6">
              <router-link to="/" class=" px-5 py-2 border border-transparent text-base leading-6 font-medium
              rounded shadow text-white bg-indigo-600 hover:bg-indigo-500 focus:outline-none focus:shadow-outline
              transitio duration-150 ease-out">
                Register
              </router-link>
            </li>
          </ul>
        </div>


      </div>
    </nav>
    <!-- End Menu Header -->

    <div class="mt-10 mx-auto max-w-screen-lg pt-20">
      <h1 class=" text-center leading-6 text-3xl tracking-tight leading-10 text-gray-900 sm:text-4xl leading-none md:text-5xl">
        Facturacion Electronica
        <span class=" text-indigo-700">simple y sensillo para tu empresa</span>
      </h1>
      <div class=" text-xl text-gray-600 mt-5 text-center px-32">
        Plausible is a lightweight and open-source website analytics tool. It doesn’t use cookies and is fully compliant
        with GDPR, CCPA and PECR.
      </div>
      <div class="text-center mt-10">
        <router-link to="/" class=" rounded-md shadow px-8 py-4 text-xl leading-6 text-white
        bg-indigo-700 font-medium hover:bg-indigo-500 focus:outline-none shadow transition duration-150">
          Iniciar Plan
        </router-link>
        <router-link to="/" class="ml-3 rounded-md shadow bg-white px-8 py-4 text-indigo-700 text-xl
         hover:text-indigo-800 ">
          Probar Demo
        </router-link>
      </div>


    </div>
    <div class="max-w-5xl mx-auto mt-24">
      <img src="@/assets/header.png" class="shadow-2xl">

    </div>
  </div>
</template>