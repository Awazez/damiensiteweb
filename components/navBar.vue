<template>
    <nav class="w-full p-6 bg-white">
      <div class="flex items-center justify-between">
  
        <!-- Header logo -->
        <div>
          <NuxtLink to="/" class="text-xl title">Damien Doussot</NuxtLink>
        </div>
  
        <!-- Mobile toggle -->
        <div class="md:hidden">
          <button @click="drawer">
            <svg 
              class="h-8 w-8 fill-current text-black"
              fill="none" stroke-linecap="round" 
              stroke-linejoin="round" stroke-width="2" 
              viewBox="0 0 24 24" stroke="currentColor">
                <path d="M4 6h16M4 12h16M4 18h16"></path>
            </svg>
          </button>
        </div>

        <!-- Navbar -->
        <div class="hidden md:block">
          <ul class="flex space-x-8 text-base font-sans">
            <li><NuxtLink to="/">Accueil</NuxtLink></li>
            <li><NuxtLink to="/qui-suis-je" >Qui suis je?</NuxtLink></li>
            <li><NuxtLink to="/accompagnement" >Accompagnement</NuxtLink></li>
            <li><NuxtLink to="/tarif" >Tarif</NuxtLink></li>
            <li><NuxtLink to="/contact" >Contact</NuxtLink></li>
          </ul>
        </div>
  
        <!-- Dark Background Transition -->
        <transition
          enter-class="opacity-0"
          enter-active-class="ease-out transition-medium"
          enter-to-class="opacity-100"
          leave-class="opacity-100"
          leave-active-class="ease-out transition-medium"
          leave-to-class="opacity-0"
        >
          <div @keydown.esc="isOpen = false" v-show="isOpen" class="z-10 fixed inset-0 transition-opacity">
              <div @click="isOpen = false" class="absolute inset-0 bg-black opacity-50" tabindex="0"></div>
          </div>
        </transition>
  
        <!-- Drawer Menu -->
        <aside class="p-5 transform top-0 left-0 w-64 bg-white fixed h-full overflow-auto ease-in-out transition-all duration-300 z-30" :class="isOpen ? 'translate-x-0' : '-translate-x-full'">
          
          <div class="close">
            <button class="absolute top-0 right-0 mt-4 mr-4" @click=" isOpen = false">
              <svg 
                class="w-6 h-6"
                fill="none" stroke-linecap="round" 
                stroke-linejoin="round" stroke-width="2"
                viewBox="0 0 24 24" stroke="currentColor">
                <path d="M6 18L18 6M6 6l12 12"></path>
              </svg>
            </button>
          </div>
  
          <span @click="isOpen = false" class="flex w-full items-center p-4 border-b">
            <NuxtLink to="/" class="text-xl title">Damien Doussot</NuxtLink>
          </span>
  
          <ul class="divide-y font-sans">
            <li><NuxtLink to="/" @click="isOpen = false" class="my-4 inline-block">Accueil</NuxtLink></li>
            <li><NuxtLink to="/qui-suis-je" @click="isOpen = false" class="my-4 inline-block">Qui suis je?</NuxtLink></li>
            <li><NuxtLink to="/accompagnement" @click="isOpen = false" class="my-4 inline-block">Accompagnement</NuxtLink></li>
            <li><NuxtLink to="/tarif" @click="isOpen = false" class="my-4 inline-block" >Tarif</NuxtLink></li>
            <li><NuxtLink to="/contact" @click="isOpen = false" class="my-4 inline-block">Contact</NuxtLink></li>
          </ul>
  
          <div class="follow">
            <p class="italic font-sans text-sm">Follow me : </p>
            <div class="social flex space-x-5 mt-4 ">
              <a href="https://www.facebook.com/profile.php?id=100087218495247">
                <svg 
                  aria-hidden="true" focusable="false" 
                  data-prefix="fab" data-icon="facebook-f" 
                  class="h-5 w-5 fill-current text-gray-600" role="img" 
                  xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512">
                  <path fill="currentColor" d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z"></path>
                </svg>
            </a>
            </div>
          </div>
  
        </aside>
  
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isOpen: false
      };
    },
    methods: {
      drawer() {
        this.isOpen = !this.isOpen;
      }
    },
    watch: {
      isOpen: {
        immediate: true,
        handler(isOpen) {
          if (process.client) {
            if (isOpen) document.body.style.setProperty("overflow", "hidden");
            else document.body.style.removeProperty("overflow");
          }
        }
      }
    },
    mounted() {
      document.addEventListener("keydown", e => {
        if (e.keyCode == 27 && this.isOpen) this.isOpen = false;
      });
    }
  };
  </script>

  <style scoped>
@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');

.title {
  font-family: 'Pacifico', cursive;
  font-size: 28px;
  margin-left: 25px;
}

</style>