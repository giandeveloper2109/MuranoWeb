<template>
    <v-footer
        style="background-color: rgb(10, 10, 50);"
      class=" text-center d-flex flex-column"
    >
      <div>
        <v-btn style="color: rgb(255, 209, 3);"
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          :icon="icon"
          variant="text"
        ></v-btn>
      </div>
  
      <div style="color: rgb(255, 209, 3);">
        Somos Murano.
      </div>
  
      <v-divider></v-divider>
  
      <div style="color: rgb(255, 209, 3);">
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
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
