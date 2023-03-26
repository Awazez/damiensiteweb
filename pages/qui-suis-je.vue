<template>
    <div>
        <CommercialBar/>
    <NavBar/><main class="pt-8 pb-16 lg:pt-16 lg:pb-24 bg-white">
  <div class="flex justify-between px-4 mx-auto max-w-screen-xl ">
      <article class="mx-auto w-full max-w-2xl format format-sm sm:format-base lg:format-lg format-blue dark:format-invert">
          <header class="mb-4 lg:mb-6 not-format">
              <address class="flex items-center mb-6 not-italic">
                  <div class="inline-flex items-center mr-3 text-sm text-gray-900 dark:text-white">
                      <img class="mr-4 w-40 h-40 rounded-full" src="@/assets/Rectangle18.png" alt="Jese Leos">
                      <div>
                          <a href="#" rel="author" class="text-xl font-bold text-gray-900">Damien Doussot</a>
                          <p class="text-base font-light text-gray-500 dark:text-gray-400">Votre psychopraticien</p>
                          <p class="text-base font-light text-gray-500 dark:text-gray-400"></p>
                      </div>
                  </div>
              </address>
              <h1 class="mb-4 text-3xl font-extrabold leading-tight text-gray-900 lg:mb-6 lg:text-4xl">Qui suis-je ? </h1>
          </header>
          <p class="lead text-justify">Dès mon plus jeune âge, j’ai eu besoin de comprendre et de mettre du sens sur 
            le fonctionnement de la vie et des comportements humains. </p> <br>
          <p class="lead text-justify">Suite à un parcours juridique dans de grandes entreprises, j’ai eu besoin de revenir à mes racines et retrouver du sens à ma vie. Je me suis 
            alors intéressé au développement personnel, à la psychologie et ouvert à la spiritualité. </p> <br>
          <p class="lead text-justify">J’ai entrepris un travail sur moi pour comprendre ma structuration, mes blocages et mes enjeux personnels. J’ai ainsi ouvert une porte merveilleuse 
            sur mon monde intérieur pour me réaliser et je continue de cheminer chaque jour en ce sens.</p> <br>
          <br>
          <p class="lead text-justify">Cela m'a permis de m'intéresser au fonctionnement de l’inconscient et aux outils pour y avoir accès. Je me suis alors formé à la psychothérapie transpersonnelle et aux états 
                modifiés de conscience afin de toucher d’autres dimensions plus profondes de l’être humain.</p> <br>
            <p class="lead text-justify">Passionné par le corps humain et son rapport à la psychologie, je me suis également formé à la sexothérapie afin de comprendre comment notre sexualité peut être le reflet 
                de nos enjeux psychiques et permettre aux femmes et aux hommes d’aller connecter leur essence.</p> <br>
                <p class="lead text-justify">Aujourd’hui, je me consacre à ce qui me fait vraiment vibrer, vous accompagner
                     à aller à la rencontre de votre monde intérieur afin que vous puissiez vous réaliser.</p> <br>
          <h2>Déontologie</h2>
          <br>
          <p class="lead text-justify">Pour aborder un domaine aussi intime et personnel que la sexualité et la vie de couple, vous avez besoin d’avoir confiance en votre thérapeute.
</p>
<br>
          <p class="lead text-justify">Le sexothérapeute est soumis au secret professionnel, ce qui signifie que ce qui se dit dans le cabinet reste dans le cabinet.</p> <br>
          <p class="lead text-justify">Lors des entretiens, le thérapeute s’abstient de formuler tout jugement quant aux confidences qui lui sont faites et accueille la personne dans son authenticité.</p> <br>
          <p class="lead text-justify">Pour les praticiens de la psychothérapie, le code de déontologie constitue un cadre de travail en énonçant plusieurs principes fondamentaux dans l’exercice de leur pratique.</p> <br>
          <p class="lead text-justify">Il se fonde sur 4 piliers:</p> <br>
          <p class="lead text-justify">- Respecter et favoriser l’autonomie de la personne qui consulte.</p> <br>
          <p class="lead text-justify">- Respecter la confidentialité des propos échangés.</p> <br>
          <p class="lead text-justify">- Développer les compétences du praticien, grâce à la formation initiale, en suivant une thérapie personnelle, en étant suivi dans sa pratique professionnelle (supervision) et en se formant en continu.</p> <br>
          <p class="lead text-justify">- Travailler en réseau afin d’orienter les personnes qui pourraient avoir besoin d’un suivi médical.​</p> <br>
          
          </article>
        </div>
        </main>
        
        </div>
</template>

<script>
export default {

}
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Ubuntu&display=swap');

h1 {
    display: flex;
    align-items: center;
    justify-content: center;
}
h2 {
    display:flex;
    align-items: center;
    justify-content: center;
    font-size: 40px;
    font-weight: 700;
}

.container-global {
    display: flex;
    align-items: center;
    justify-content: center;
}

.container-left {
    font-size: 24px;
    width: 600px;
    height: 200px;
    margin:auto;
}

.container-right{
    margin-left: 50px;
    font-size: 24px;
    text-align: justify;

}

.container-text {
    padding-top: 50px;
    width: 100%;
    height: 500px;
    font-size: 35px;
    border: none;
    background-color: #111827;
    color: white;
    text-align: center;
}

.container-title {
    width: 1000px;
    margin: auto;
}

.container-perso {
    margin: auto;
    width: 1000px;
    height: 1000px;
    padding-top: 100px;
    padding: 100px;
    background-color: white;
    margin-left: 50px;
    font-size: 24px;
    text-align: justify;
}

@media only screen and (max-width : 420px) {
/* Styles */

h2 {
    display:flex;
    align-items: center;
    justify-content: center;
    font-size: 40px;
    font-weight: 700;
}

.container-global {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.container-left {
    font-size: 14px;
    width: auto;
    height: auto;
    display: flex;
    align-content: center;
    justify-content: center;
    margin: auto;
    background-color: red;
}

.container-right{
    margin-top: 100px;
    font-size: 24px;
    text-align: justify;
    background-color: blue;

}
}


</style>
