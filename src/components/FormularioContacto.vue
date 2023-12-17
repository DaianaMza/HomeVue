<template>
    <div>
      <div class="container mx-auto my-4 px-4 lg:px-20">
        <div class="w-full p-8 my-4 md:px-12 lg:w-9/12 lg:pl-20 lg:pr-40 mr-auto rounded-2xl shadow-2xl">
          <div class="flex">
            <h1 class="font-bold uppercase text-5xl text-white">Contactanos!</h1>
          </div>
          <form @submit.prevent="handleSubmit">
            <div class="grid grid-cols-1 gap-5 md:grid-cols-2 mt-5">
              <input
                class="w-full bg-gray-100 text-gray-900 mt-2 p-3 rounded-lg focus:outline-none focus:shadow-outline"
                type="text"
                placeholder="Nombre"
                v-model="name"
              />
              <input
                class="w-full bg-gray-100 text-gray-900 mt-2 p-3 rounded-lg focus:outline-none focus:shadow-outline"
                type="email"
                placeholder="Email"
                v-model="email"
              />
            </div>
            <select
              class="w-full bg-gray-100 text-gray-900 mt-2 p-3 rounded-lg focus:outline-none focus:shadow-outline"
              aria-label="Default select example"
              v-model="subject"
            >
              <option value="none">Asunto</option>
              <option value="Consultoria">Consultoria</option>
              <option value="Auditoria">Auditoria</option>
              <option value="Formacion y Capacitacion">Formacion y Capacitacion</option>
              <!-- <option value="Otros Servicios">Otros Servicios</option> -->
            </select>
            <div class="my-4">
              <textarea
                placeholder="Mensaje"
                class="w-full h-32 bg-gray-100 text-gray-900 mt-2 p-3 rounded-lg focus:outline-none focus:shadow-outline"
                v-model="message"
              ></textarea>
            </div>
            <div class="my-2 w-1/2 lg:w-1/4">
              <button
                type="submit"
                class="uppercase text-sm font-bold tracking-wide bg-blue-900 text-gray-100 p-3 rounded-lg w-full focus:outline-none focus:shadow-outline"
              >
                Enviar Mensaje
              </button>
            </div>
          </form>
        </div>
  
        <div class="w-full lg:-mt-96 lg:w-2/6 px-8 py-12 ml-auto bg-blue-900 rounded-2xl">
          <div class="flex flex-col text-white">
            <div class="flex my-4 w-2/3 lg:w-1/2">
              <div class="flex flex-col">
                <i class="fas fa-map-marker-alt pt-2 pr-2" />
              </div>
              <div class="flex flex-col">
                <h2 class="text-2xl">Oficina:</h2>
                <p class="text-gray-400">Rodríguez Peña 95 depto 8Q CABA</p>
              </div>
            </div>
  
            <div class="flex my-4 w-2/3 lg:w-1/2">
              <div class="flex flex-col">
                <i class="fas fa-phone-alt pt-2 pr-2" />
              </div>
              <div class="flex flex-col">
                <h2 class="text-2xl">Telefono:</h2>
                <p class="text-gray-400">Tel: +54 911 5955 4409</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        email: '',
        subject: 'none',
        message: '',
      };
    },
    methods: {
      handleSubmit() {
        const mailtoLink = `mailto:ejemplo@gmail.com?subject=${encodeURIComponent(
          this.name + ' ' + this.subject
        )}&body=${encodeURIComponent(this.message)}`;
        window.location.href = mailtoLink;
      },
    },
  };
  </script>
  
  <style scoped>
  </style>
  