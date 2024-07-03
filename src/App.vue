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
import EnterpriseLogoHorizontalDark from './assets/logo-horizontal-dark.png'
</script>

<template>
  <ContactBar email="contato@edificcontrutora.com" telephone="(44) 999915783" instagram="/edific.construtora"/>

  <div class="first-page-container">
      <img :src="EnterpriseLogoHorizontalDark" alt="logo">
      <div class="first-page-text-container">
        <span class="first-page-title">QUALIDADE E AGILIDADE NO MERCADO DA PERÍCIAS, AVALIAÇÕES E DIAGNÓSTICOS DAS EDIFICAÇÕES</span>
        <span class="first-page-subtitle">Perícias, avaliações e diagnósticos das edificações</span>
      </div>
      <QueroContratarButton class="first-page-button"/>
  </div>

  <div class="second-page-container">
    <h2>Serviços da Engenharia Diagnóstica</h2>
    <Card class="second-page-first-card" title="Laudo estrutural:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
    <div class="second-page-cards-container">
      <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="VISTORIA CAUTELAR DE VIZINHANÇA:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="AVALIAÇÃO DE IMÓVEIS:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
      <Card title="INSPEÇÃO PREDIAL:" subtitle="O Laudo Cautelar de Vizinhança ou simplesmente Laudo de Vizinhança, é o documento que visa evitar conflitos desnecessárias em casos de danos causados por uma obra em imóveis localizados em seu entorno."/>
    </div>
  </div>

  <div class="third-page-container">
    <div class="third-page-text-container">
      <h2>EDIFIC CONSTRUTORA</h2>
      <p>Realizamos o diagnóstico em edificações buscando garantir a sua integridade e atribuindo soluções aos problemas construtivos, sejam estes originados na fase de projetos, durante a execução da obra, por carência de manutenção, em função de vícios construtivos, ou ainda, em razão de sinistros.</p>
      <p>Com objetivo de ser referência no mercado da perícia técnica e diagnóstica, a Edific Construtora visa priorizar a segurança, a durabilidade e habitabilidade das edificações, além de, atentar a saúde e o bem estar de seus usuários.</p>
      <p>Possuímos equipes especializadas, buscamos todas as atualizações tecnológicas, além de seguir com rigor as normas da associação brasileira de normas técnicas (ABNT).</p>
    </div>
    <QueroContratarButton class="third-page-button"/>
  </div>

  <div class="fourth-page-container">
    <h2>PORQUE ESCOLHER TAB ENGENHARIA</h2>
    <div class="fourth-page-cards-container">
      <Card2 :image="image0" description="Possuímos corpo de engenharia especializado em engenharia diagnóstica para garantir as melhores soluções técnicas."/>
      <Card2 :image="image0" description="Única empresa do Paraná a pertencer ao comitê da construção civil -ABNT."/>
      <Card2 :image="image0" description="Membros da divisão técnica de engenharia diagnóstica."/>

      <Card2 :image="image0" description="Empresa membro da ADPAT – Academia da patologia ."/>
      <Card2 :image="image0" description="Empresa especialista em atendimento condominial."/>
      <Card2 :image="image0" description="Empresa registrada no TJPR (Perita judicial)."/>
    </div>
    
    <QueroContratarButton class="fourth-page-button"/>
  </div>

  <div class="fifth-page-container">

</div>

  
  <!--<BottomBar :enterpriseLogo="EnterpriseLogo" whatsapp="(11) 97178-2034" email="comercial@tabengenharia.com.br" instagram="@tabengenharia"/>-->  
  <!-- <Card2 :image="image0" description="Possuímos corpo de engenharia especializado em engenharia diagnóstica para garantir as melhores soluções técnicas."/> -->
  <!-- 
  <LocalCard title="LOCAL 2" subtitle="R. São Cristóvão, 57 – ZONA 8 – Zona 08, Maringá – PR, 87050-490" telephone="(43) 99987-5018" :image="image2"/>
  <QueroContratarButton/> -->
</template>

<style scoped>
.first-page-container{
  display: flex;
  flex-direction: column;
  height: 670px;
  justify-content: center;
  align-items: center;
  position: relative;
  background-image: url('./assets/first-page-background.fw.png');
  background-repeat: no-repeat;
  background-size: cover;
}
.first-page-container > img{
  max-width: 400px;
  position: absolute;
  top: 0;
  margin-top: 80px;
}
.first-page-text-container{
  max-width: 850px;
  display: flex;
  flex-direction: column;
  padding: 0px 20px;
}
.first-page-title{
  font-size: 40px;
  font-weight: 600;
  color: #fff;
  text-transform: uppercase;
  line-height: 1;
  margin-bottom: 10px;
  text-align: center;
}
.first-page-subtitle{
  text-align: justify;
  color: #fff;
  font-size: 17px;
  text-align: center;
}
.first-page-button{
  position: absolute;
  bottom: 0;
  margin-bottom: 140px;
}
@media (max-width: 760px) {
  .first-page-container{
    height: fit-content;
  }
  .first-page-title{
    font-size: 32px;
    line-height: 1.2em;
  }
  .first-page-container > img{
    margin-top: 0;
    position: initial;
    margin-bottom: 14px;
    max-width: 400px;
    width: 80vw;
    margin-top: 40px;
  }
  .first-page-button{
    position: initial;
    margin-bottom: 0;
    margin-top: 36px;
    margin-bottom: 50px;
  }
}
/* ----------------------------------------------- */
.second-page-container{
  display: flex;
  flex-direction: column;
  align-items: center;

  display: none;
}
.second-page-container > h2{
  color: #282828;
  font-size: 35px;
  font-weight: 600;
  margin-top: 60px;
  margin-bottom: 36px;
}
.second-page-first-card{
  max-width: 700px;
}
.second-page-cards-container{
  display: grid;
  gap: 20px;
  grid-template-columns: repeat(3, 1fr);
}
/* ----------------------------------------------- */
.third-page-container{
  background-color: red;
  display: flex;
  flex-direction: column;
  align-items: center

}
.third-page-text-container{
  max-width: 680px;
  padding: 50px 20px;
  padding-bottom: 30px;
}
.third-page-text-container > h2{
  color: #fff;
  font-size: 45px;
  font-weight: 600;
  line-height: 46px;
  margin-bottom: 20px;
}
.third-page-text-container > p{
  text-align: justify;
  color: #fff;
  font-size: 17px;
  margin-top: 10px;
}
.third-page-button{
  margin-bottom: 36px;
}
@media (max-width: 547px) {
  .third-page-text-container > h2{
    font-size: 35px;
    text-align: center;
  }
}
/* ----------------------------------------------- */
.fourth-page-container{
  background-image: url('./assets/curitiba-do-alto-guilherme-pupo-2.fw.png');
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.fourth-page-container > h2{
  color: #fff;
  font-size: 40px;
  font-weight: 600;
  text-align: center;
  padding: 0px 16px;
  padding-top: 50px;
  padding-bottom: 26px;
}
.fourth-page-cards-container{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  max-width: 810px;
  gap: 16px;
  padding: 0px 10px;
}
.fourth-page-button{
  margin: 36px 0px;
}
@media (max-width: 820px) {
  .fourth-page-cards-container{
    grid-template-columns: repeat(1, 1fr);
    width: fit-content;
    gap: 5px;
  }
  .fourth-page-button{
    margin-top: 20px;
  }
}
@media (max-width: 420px) {
  .fourth-page-cards-container{
    gap: 20px;
  }
}



</style>
