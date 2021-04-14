<template>
  <nav class="flex items-center bg-gray-800 p-3 flex-wrap">
    <div>
      <a
        href="#"
        class="p-2 mr-4 inline-flex items-center text-white text-3xl font-bold uppercase tracking-wide  "
        >NAVBAR</a
      >
    </div>

    <div class="ml-auto">
      <!-- lg:hidden hides the menu icon on large screens -->
      <button
        class="inline-flex p-3 text-white hover:bg-gray-900 rounded lg:hidden"
        @click="showMenu()"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
      </button>
    </div>

    <!-- Small screen navigation -->'
   
    
        <div
      class="w-full lg:inline-flex lg:flex-grow lg:w-auto lg:hidden" v-if="toggleMenu"
      id="navigation"
    
    >
      <div class="lg:inline-flex lg:flex-row lg:ml-auto flex flex-col ">
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white w-16"
          >Home</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white w-16 "
          >FQAs</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white w-48"
          >Passport Registration</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white w-48"
          >Ecommerce Providers</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white w-48"
          >Order Now</a
        >
      </div>
    </div>
    
    <div
      class="w-full lg:inline-flex lg:flex-grow lg:w-auto sm:hidden" 
      id="navigation"
      
    >
      <div class="lg:inline-flex lg:flex-row lg:ml-auto flex flex-col ">
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white"
          >Home</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white"
          >FQAs</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white"
          >Passport Registration</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white"
          >Ecommerce Providers</a
        >
        <a
          href="#"
          class="lg:inline-flex lg:w-auto px-3 py-2 rounded text-gray-400 hover:bg-gray-900 hover:text-white"
          >Order Now</a
        >
      </div>
    </div>
    
  </nav>
</template>

<script>
export default {
  data() {
    return {
      toggleMenu: false,
    };
  },
  methods: {
    showMenu() {
      this.toggleMenu = !this.toggleMenu;
    },
  },
};
</script>

