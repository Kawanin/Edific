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
  <ContactBar email="contato@edificcontrutora.com" telephone="(44) 999915783" instagram="/tabengenharia"/>
  <!--<BottomBar :enterpriseLogo="EnterpriseLogo" whatsapp="(11) 97178-2034" email="comercial@tabengenharia.com.br" instagram="@tabengenharia"/>-->  
  <!-- <Card2 :image="image0" description="Possuímos corpo de engenharia especializado em engenharia diagnóstica para garantir as melhores soluções técnicas."/> -->
  <!-- 
  <LocalCard title="LOCAL 2" subtitle="R. São Cristóvão, 57 – ZONA 8 – Zona 08, Maringá – PR, 87050-490" telephone="(43) 99987-5018" :image="image2"/>
  <QueroContratarButton/>
  <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/> -->
</template>

<style scoped>
</style>
