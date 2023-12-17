<template>
    <div class="w-full px-5 py-16 md:py-24 text-gray-800">
      <div class="w-full max-w-6xl mx-auto">
        <div class="text-center max-w-xl mx-auto">
          <h1 class="text-6xl md:text-7xl font-bold mb-5 text-white">Nuestros Servicios</h1>
          <div class="text-center mb-10">
            <span class="inline-block w-1 h-1 rounded-full bg-indigo-500 ml-1"></span>
            <span class="inline-block w-3 h-1 rounded-full bg-indigo-500 ml-1"></span>
            <span class="inline-block w-40 h-1 rounded-full bg-indigo-500"></span>
            <span class="inline-block w-3 h-1 rounded-full bg-indigo-500 ml-1"></span>
            <span class="inline-block w-1 h-1 rounded-full bg-indigo-500 ml-1"></span>
          </div>
        </div>
        <v-tabs v-model="tabIndex" color="indigo" background-color="white" centered>
          <v-tab v-for="(label, index) in tabLabels" :key="index" :href="'#tabpanel-' + index">
            {{ label }}
          </v-tab>
        </v-tabs>
        <v-tab-item v-for="(component, index) in tabComponents" :key="index" :value="index">
          <v-box v-if="tabIndex === index" p="3">
            <component :is="component" />
          </v-box>
        </v-tab-item>
      </div>
    </div>
  </template>
  
  <script>
  /* eslint-disable vue/multi-word-component-names */
  import Uno from "../components/Services/Service1";
  import Dos from "../components/Services/Service2";
  import Tres from "../components/Services/Service3";
  
  export default {
    data() {
      return {
        tabIndex: 0,
        tabLabels: ["Consultoria", "Auditoria", "Formacion y Capacitacion"],
        tabComponents: [Uno, Dos, Tres],
      };
    },
  };
  </script>
  
  <style scoped>
  /* Add your component-specific styles here */
  </style>
  