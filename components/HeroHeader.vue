<template>
<section class="bg-white background">
  <div class="mx-auto max-w-screen-xl px-4 py-8 lg:flex lg:h-screen lg:items-center">
    <div class="mx-auto max-w-xl text-center">
      <h1 class="text-3xl font-extrabold sm:text-5xl">
        Pour retrouver confiance en soi et plénitude
      </h1>

      <p class="mt-4 sm:text-xl sm:leading-relaxed">
        Damien Doussot, psychopraticien vous reçoit dans son cabinet, en visio ou lors d’ateliers et stages
      </p>

      <div class="mt-8 flex flex-wrap justify-center gap-4 pb-10">
        <a
          class="block w-full rounded bg-[#111827] px-12 py-3 text-sm font-medium text-white shadow hover:bg-gray-700  focus:outline-none focus:ring active:bg-black sm:w-auto"
          href="https://calendly.com/damien-doussot-therapeute"
        >
          Prendre RDV
        </a>

        <a
          class="block w-full rounded bg-[#111827] px-12 py-3 text-sm font-medium text-white shadow hover:bg-gray-700  focus:outline-none focus:ring active:bg-black sm:w-auto"
          href="/contact"
        >
          Contact
        </a>
      </div>
    </div>
  </div>
</section>
</template>
    
<script>
    export default {
    }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@800&display=swap');



h1 {
  font-family: 'Lato', sans-serif;
  color: black;
  font-size: 3em;
  font-weight:bold; 
}
p {
  font-size: 1.5rem;
  margin: 0 1.25rem 5rem 1.25rem;
  color: black;
}

span {
  display: inline-block;
}

.box{
    width:200px; 
    height:50px; 
    background: #ccc; 
    margin: 0 auto; 
    text-align:center; 
    line-height:50px;
}

.clip-path {
  width: 100%;
  min-height: 600px;
  clip-path: polygon(0 0, 100% 0, 100% 92%, 0 100%);
}

.hero_title {
    font-family: 'Raleway', sans-serif;
    font-size: 50px;
    color: white;
}
.fadeInUp{
    animation:fadeInUp 0.5s ease backwards;
    margin-left: 8px;
}

@keyframes fadeInUp{
  0%{transform:translate(0px, 30px); opacity: 0;}
  100%{transform:translate(0px, 0); opacity: 1;}
}


@media only screen and (max-width: 768px){
.hero_title {
    font-size: 50px;
  }
}

    
</style>

