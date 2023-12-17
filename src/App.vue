<script>
import './assets/tailwind.css'
import HeroHeader from './components/HeroHeader.vue';
import NavbarIndex from './components/NavbarIndex.vue';
import QuienesSomos from './components/QuienesSomos.vue'
import NuestroServicio from './components/NuestroServicio.vue'
import NuestrosClientes from './components/NuestrosClientes.vue'
import FormularioContacto from './components/FormularioContacto.vue'
import Footer from './components/Footer.vue'
import styles from './styles'

const { boxWidth, paddingX, flexCenter, flexStart } = styles;

export default {
  name: 'App',
  components: { NavbarIndex, HeroHeader,QuienesSomos,NuestroServicio , NuestrosClientes, FormularioContacto,Footer},
  data() {
    return {
      boxWidth,
      paddingX,
      flexCenter,
      flexStart
    };
  },
};
</script>


<template>
  <div class="bg-blue-950 w-full overflow-hidden">
    <div :class="['bg-blue-950', paddingX, flexCenter]">
      <div :class="[boxWidth]">
        <NavbarIndex />
      </div>
    </div>
    <div :class="['bg-blue-950', flexStart]">
      <div :class="[boxWidth]">
        <HeroHeader />
      </div>
    </div>

    <div :class="[flexStart]">
      <div :class="[boxWidth]">
        <QuienesSomos />
        <NuestroServicio />
        <NuestrosClientes/>
        <FormularioContacto/>
        <Footer/>
      </div>
    </div>

  </div>
</template>



<style></style>
