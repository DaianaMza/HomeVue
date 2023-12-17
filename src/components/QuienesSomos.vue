<script>
import styles from '../styles'

const { flexCenter,paddingY,} = styles;
export default {
    data() {
        return {
            paddingY,flexCenter,
    
        };
    },
};
</script>

<template>
    <div>
        <section id="home" :class="[paddingY, 'flex md:flex-row flex-col',flexCenter]">
          <div className="container flex flex-col items-center p-4 mx-auto space-y-6 md:p-8">
            <h1 className="px-6 py-2 text-2xl font-semibold text-center sm:font-bold sm:text-3xl md:text-4xl lg:max-w-2xl xl:max-w-4xl text-white">Sobre Nosotros:</h1>
            <p className="px-6 py-2 text-2xl font-semibold text-center sm:font-bold sm:text-3xl md:text-4xl lg:max-w-2xl xl:max-w-4xl text-white">"Somos un grupo multidisciplinario busca aumentar la competitividad y crecimiento integral de nuestros clientes en materia de excelencia de la calidad,
              seguridad y sustentabilidad. La diversificación de nuestros servicios permite que nuestros clientes tengan la confianza de contar con un soporte profesional integral"</p>
          </div>
        </section>
      </div>
</template>
  

  
<style scoped></style>