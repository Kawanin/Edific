<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import QueroContratarButton from './components/QueroContratarButton.vue'
import Card from './components/Card.vue'
import LocalCard from './components/LocalCard.vue'
import image2 from "./assets/mapa2.webp"
import ContactBar from './components/ContactBar.vue'
import Card2 from './components/Card2.vue'
import image0 from './assets/tab1.webp'
import BottomBar from './components/BottomBar.vue'
import EnterpriseLogo from './assets/logo-tab.png'
</script>

<template>
<!--   <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView /> -->

  <BottomBar :enterpriseLogo="EnterpriseLogo" whatsapp="(11) 97178-2034" email="comercial@tabengenharia.com.br" instagram="@tabengenharia"/>
  <!-- <Card2 :image="image0" description="Possuímos corpo de engenharia especializado em engenharia diagnóstica para garantir as melhores soluções técnicas."/> -->
  <!-- <ContactBar email="contato@edificcontrutora.com" telephone="(44) 999915783" instagram="/tabengenharia"/>
  <LocalCard title="LOCAL 2" subtitle="R. São Cristóvão, 57 – ZONA 8 – Zona 08, Maringá – PR, 87050-490" telephone="(43) 99987-5018" :image="image2"/>
  <QueroContratarButton/>
  <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/> -->
  

</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

*{
  font-family: "Poppins", Sans-serif;
}
</style>

<style scoped>


/* header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
} */
</style>
