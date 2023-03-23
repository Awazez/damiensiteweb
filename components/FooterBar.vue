<template>
   
   <section class="bg-white">
    <div class="max-w-screen-xl px-4 py-12 mx-auto space-y-8 overflow-hidden sm:px-6 lg:px-8">
        <nav class="flex flex-wrap justify-center -mx-5 -my-2">
            <div class="px-5 py-2">
                <NuxtLink to="/" class="text-base leading-6 text-gray-500 hover:text-gray-900">
                    Accueil
                </NuxtLink>
            </div>
            <div class="px-5 py-2">
                <NuxtLink to="/qui-suis-je" class="text-base leading-6 text-gray-500 hover:text-gray-900">
                    Qui Suis Je ?
                </NuxtLink>
            </div>
            <div class="px-5 py-2">
                <NuxtLink to="/accompagnement" class="text-base leading-6 text-gray-500 hover:text-gray-900">
                    Accompagnement
                </NuxtLink>
            </div>
           

            <div class="px-5 py-2">
                <NuxtLink to="/tarif" class="text-base leading-6 text-gray-500 hover:text-gray-900">
                    Tarifs 
                </NuxtLink>
            </div>
         
            <div class="px-5 py-2">
                <NuxtLink to="/contact" class="text-base leading-6 text-gray-500 hover:text-gray-900">
                    Contact
                </NuxtLink>
            </div>
        
        </nav>
        <div class="flex justify-center mt-8 space-x-6">
            <a href="https://www.facebook.com/profile.php?id=100087218495247" class="text-gray-400 hover:text-gray-500">
                <span class="sr-only">Facebook</span>
                <svg class="w-6 h-6" aria-hidden="true" fill="currentColor" viewBox="0 0 24 24">
                    <path fill-rule="evenodd" d="M22 12c0-5.523-4.477-10-10-10S2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094 0 2.238.195 2.238.195v2.46h-1.26c-1.243 0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12z" clip-rule="evenodd"></path>
                </svg>
            </a>
        </div>
        <p class="mt-8 text-base leading-6 text-center text-gray-400">
            Fait avec ❤️ en Normandie
        </p>
    </div>
</section>

</template>

<script>
export default {
    
}


</script>

<style scoped>

@import url('https://fonts.googleapis.com/css?family=Open+Sans');

h1 {
    color: dim-black;
}

h2 {
    color: white;
}

h3 {
    color: white;
    font-size: 50px;
}

  .wave-container {
  position: relative;
  background-color: black;
  color: black;
  text-align: center;
  overflow: hidden;
}

.footer{
    margin-top: 100px;
    float:left;
    width:100%;
    line-height: 60px;
    height:400px;
    clip-path: polygon(0 9%, 100% 0, 100% 100%, 0% 100%);
}

</style>