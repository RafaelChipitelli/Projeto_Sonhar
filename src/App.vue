<script setup>
  import { reactive } from 'vue';
  import Cabecalho from './components/Cabecalho.vue'
  import SobreNos from './components/SobreNos.vue'
  import Projetos from './components/Projetos.vue'
  import Membros from './components/Membros.vue'
  import Carousel from './components/Carousel.vue';
  import Voluntario from './components/Voluntario.vue';
  

  const whatsappNumber = 'https://wa.me/5521988112805?text=Ol%C3%A1+Vim+do+Site';
</script>

<template>
  <Cabecalho/>
  <Carousel/>
  <SobreNos/>
  <Projetos/>
  <Membros/>
  <Voluntario/>
  
  <a :href="whatsappNumber" target="_blank" class="whatsapp-button">
    <i class="fab fa-whatsapp"></i>
  </a>
</template>

<style scoped>
.whatsapp-button {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #25d366;
    color: #fff;
    width: 60px;
    height: 60px;
    border: none;
    border-radius: 50%;
    font-size: 24px;
    cursor: pointer;
    transition: background-color 0.3s ease;
    text-decoration: none;
    display: flex;
    align-items: center;
    justify-content: center;
}

.whatsapp-button i {
    /* Mantenha os estilos anteriores */

    margin: 0; /* Remova as margens padrão do ícone */
}

.whatsapp-button:hover {
    background-color: #128c7e;
}
</style>


