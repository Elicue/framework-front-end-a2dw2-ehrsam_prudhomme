<script setup>
import Connect from './components/Connect.vue';
import Card from './components/Card.vue';
import Boutton from './components/Boutton.vue';
import Pages from './components/Pages.vue';
import DropDownFooter from './components/DropDownFooter.vue';
import IconeCard from './components/IconeCard.vue';
import FooterCat from './components/FooterCat.vue';

</script>

<template>
  <div class="flex flex-col overflow-x-hidden items-center relative w-screen h-screen">
  <header class="block relative  w-screen items-center text-white">
    <img class="h-full md:h-auto top-0 absolute w-full -z-10" src="../fond.png" alt="fond">
    
    <nav class="md:flex hidden flex-row w-11/12 md:h-30 h-32 justify-between items-center mx-auto">
      <div class="w-1/2 flex flex-row justify-around items-center">
        <img class="hidden md:flex w-30 h-4" src="../logo.svg" alt="logo">
        <div class="w-2/3 hidden md:flex flex-row justify-around">
          <p>Offres</p>
          <p class="font-semibold">Formation</p>
          <p>Ressources</p>
          <p>A propos</p>
        </div>
      </div>

      <div class=" w-1/4 hidden md:flex font-semibold justify-around">
        <Boutton class="bg-white/30" msg="06 74 49 03 21"/>
        <Boutton class=" text-purple bg-white" msg="Je prends contact"/>
      </div>
    </nav>

    <nav class="flex md:hidden h-20 items-center w-11/12 mx-auto">
      <div class="md:hidden flex flex-row justify-between w-screen">
        <img class="flex h-8" src="../Logotypes Skillsday.svg" alt="logo">
        <img class="flex" src="../menu.svg" alt="menu">
      </div>
    </nav>

    <div class=" md:mt-5 mt-6 mb-20 flex flex-col text-center items-center">
      <h1 class="md:text-6xl text-3xl md:w-auto w-11/12 font-bold mb-10">Découvrez nos formations sur étagère ! </h1>
      <p class=" md:w-1/2 mx-auto -mt-5 md:mt-0 w-11/12">Notre catalogue de formations soft skills est le meilleur allié de vos managers et collaborateurs. Management, vente, ressources humaines, efficacité professionnelle... Composez votre parcours de formation et mixez les modalités pédagogiques pour développer leurs compétences.</p>
    </div>
  </header>

  <div class="md:mt-4 -mt-12 translate-2/4 p-5 rounded-3xl w-11/12 md:w-9/12 mx-auto flex md:flex-row flex-col justify-around bg-white text-font shadow-lg">
    <div class="rounded-full py-2 px-5 w-full md:w-9/12 flex flex-row bg-light_purple justify-between items-center ">
      <p class="md:flex hidden">Quelle formation recherchez-vous ?</p>
      <p  class="md:hidden flex">Quelle formation recherch...</p>
      <img class=" w-8" src="../search.svg" alt="search">
    </div>
    
    <div class=" mt-5 md:mt-0 rounded-full py-2 px-10 w-full md:w-2/12 flex flex-row bg-light_purple md:justify-around justify-between items-center">
      <p>Filtrer </p>
      <img src="../down.svg" alt="down">
    </div>
  </div>

  <main class="md:mt-20 mt-20 w-11/12 mx-auto flex flex-col justify-between " >

    <div class="flex flex-row w-maw justify-between items-center mb-10">
      <h3 class="text-lg font-semibold uppercase">Les PLUS POPULAIRES 🔥</h3>
      <div class="flex flex-row items-center">
        <img class="w-6 h-6" src="../arrow_l.svg" alt="arrow">
        <img class="w-6 h-6 ml-2" src="../arrow_r.svg" alt="arrow">
      </div>
    </div>

    <div class="justify-between grid md:grid-cols-4 gap-6">
        <Card url="/Intersect.jpg">
          <template v-slot:title>
            <p class="uppercase text-xs">Management & Leadership</p>
          </template>
          <template v-slot:icone>
            <IconeCard/>
            <IconeCard/>
            <IconeCard/>
          </template>
        </Card>

        <Card url="/Intersect.png">
          <template v-slot:title>
            <p class="uppercase text-xs">Vente</p>
          </template>
          <template v-slot:icone>
            <IconeCard/>
          </template>
        </Card>

        <Card url="/Intersect2.png">
          <template v-slot:title>
            <p class="uppercase text-xs">RH, QVT & diversité</p>
          </template>
          <template v-slot:icone>
            <IconeCard/>
            <IconeCard/>
          </template>
        </Card>

        <Card url="/Intersect3.png">
          <template v-slot:icone>
            <IconeCard/>
            <IconeCard/>
            <IconeCard/>
          </template>
        </Card>

    </div>
  </main>

  <main class="-mb-5 mb:mt-40 mt-20 w-11/12 mx-auto flex flex-col justify-between" >
    <h3 class="text-lg font-semibold uppercase mb-10">TOUTES LES FORMATIONS 🚀</h3>

    <div class="justify-between md:mb-16 grid md:grid-cols-4 gap-6">
      <Card url="/Intersect1-1.png">
        <template v-slot:icone>
          <IconeCard/>
          <IconeCard/>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect1-2.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect1-3.png">
        <template v-slot:icone>
          <IconeCard/>
          <IconeCard/>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect1-4.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>
    </div>

    <div class="justify-between md:mb-16 grid md:grid-cols-4 gap-6">
      <Card url="/Intersect2-1.png">
        <template v-slot:icone>
          <IconeCard/>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect2-2.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect2-3.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect2-4.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>
    </div>

    <div class="justify-between grid md:grid-cols-4 gap-6">
      <Card url="/Intersect3-1.png">
        <template v-slot:icone>
          <IconeCard/>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect3-2.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect3-3.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>

      <Card url="/Intersect3-4.png">
        <template v-slot:icone>
          <IconeCard/>
        </template>
      </Card>
    </div>

  </main>

    <div class="w-screen flex justify-end md:-ml-32">
      <div class="md:mt-20 mt-8 relative flex flex-row justify-between w-48 items-center md:mx-0 mx-auto">
        <Pages class="flex text-border_IconeCard opacity-100 border-2 rounded-full w-10 h-10 items-center pl-3 border-border_IconeCard text-2xl" number="1"/>
        <Pages number="2"/>
        <Pages number="3"/>
        <Pages number="4"/>
        <Pages number="..."/>
        <Pages number="8"/>
      </div>
    </div>
    <div class="mt-20 md:w-7/12 w-11/12 items-center md:h-60 justify-around mx-auto flex flex-col bg-light_purple rounded-2xl py-5 text-center">
      <h3 class="my-5 md:text-3xl text-2xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-blue via-purple to-border_IconeCard md:text-black">C’est votre dernier mot ?</h3>
      <p class="md:w-5/12 w-11/12 ">Si vous n’avez pas trouvé ce que vous cherchez, dites-le nous.</p>
      <div class="my-5 flex md:flex-row flex-col w-11/12 md:w-6/12 justify-between items-center">
        <Boutton class="bg-purple hover:scale-105 transition-all text-white h-14 font-semibold w-full md:w-auto" msg="Je prends contact"/>
        <div class="bg-[url('/fond.png')] hover:scale-105 transition-all h-14 bg-cover rounded-full items-center flex px-1 mt-5 md:mt-0 w-full md:w-auto">
          <Boutton class=" w-full  h-12 md:mt-0 font-semibold border-2 bg-light_purple" msg="Télécharger le catalogue"/>
        </div>
      </div>
    </div>

  <footer class="mt-20 relative w-screen md:pb-20 -pb-10 flex flex-col bg-font text-white bottom-0 md:pl-20">  

    <div class="flex md:flex-row flex-col mt-28 mb-20">
      <div>
      
        <img class="mb-5 pl-5" src="../Logotypes Skillsday.svg" alt="skillsday">
        <p class="md:flex  hidden pl-5 w-60" >Skillsday est un organisme nouvelle génération qui a pour mission de moderniser et digitaliser la formation en entreprise pour former, vraiment !</p>
        <p class="md:hidden  flex pl-5 w-11/12 ">Skillsday, l’agence du mobile learning qui accompagne la performance des collaborateurs sur des formats courts, ciblés et efficients.</p>
      </div>
      
      <DropDownFooter titre="solutions"/>
      <DropDownFooter titre="formations"/>
      <DropDownFooter titre="informations"/>

      <FooterCat>
        <template v-slot:title>
          <h4 class="opacity-40 uppercase mb-5">solutions</h4>
        </template>
        <template v-slot:text>
          <p class="mb-2">Développer les soft skills</p>
          <p class="mb-2">Digitaliser les formations</p>
          <p class="mb-2">Accompagner les déploiements</p>
        </template>
      </FooterCat>

      <FooterCat>
        <template v-slot:title>
          <h4 class="opacity-40 uppercase mb-5">formations</h4>
        </template>
        <template v-slot:text>
          <p class="mb-2">Toutes les formations</p>
          <p class="mb-2">Télécharger le catalogue</p>
        </template>
      </FooterCat>

      <FooterCat>
        <template v-slot:title>
          <h4 class="opacity-40 uppercase mb-5">informations</h4>
        </template>
        <template v-slot:text>
          <p class="mb-2">Nous rejoindre</p>
          <p class="mb-2">Nous contacter</p>
          <p class="mb-2">FAQ</p>
        </template>
      </FooterCat>

    </div>
    <div class="flex md:flex-row flex-col">
      <div class=" ml-5  flex flex-col">
        <p>©Skillsday 2022</p>
        <div class="mt-5 flex md:flex-row flex-col justify-between h-32 w-full">
          <p>Mentions légales</p>
          <P class="md:flex hidden mx-2">•</P>
          <p>Politique de confidentialité</p>
          <P class="md:flex hidden mx-2">•</P>
          <p>CGV</p>
        </div>
      </div>

      <div class="mb-5 flex flex-row justify-between md:w-2/12 w-1/2  ml-30 mt-16 md:mt-0 md:ml-20 mx-auto">
      
        <Connect urlConnect="/instagram.svg"/>
        <Connect urlConnect="/linkedin.svg"/>
        <Connect urlConnect="/frame.svg"/>
        <Connect urlConnect="/youtube.svg"/>

      </div>
    </div>

  </footer>
  </div>
</template>

<style scoped>
</style>
