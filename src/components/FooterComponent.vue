<template>
    <v-footer
        style="background-color:#000744 ;"
      class=" text-center d-flex flex-column"
    >
      <div>
        <v-btn style="color: #f4a414;"
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          :icon="icon"
          variant="text"
        ></v-btn>
      </div>
  
      <div style="color: #f4a414;">
        Somos Murano.
      </div>
  
      <v-divider></v-divider>
  
      <div style="color: #f4a414;">
        {{ new Date().getFullYear() }} — <strong>Inmobiliaria Murano Investment S.A.C </strong>
      </div>
    </v-footer>
  </template>
  <script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>
