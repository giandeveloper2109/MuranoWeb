<template>
  <v-app-bar  flat app class=" text-center d-flex flex-column">
    <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
    <div>
      <router-link to="/">
        <v-img  class="mr-3" src="@/assets/logoMurano.png" height="200px" width="200px"></v-img>
      </router-link>
      
    </div>
    <v-spacer></v-spacer>
    <div>
      <v-btn to="/"  style="color: rgba(11, 31, 145, 0.772);">Home</v-btn>
    </div>
    <v-divider  :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-btn to="/contactanos" text style="color: rgba(11, 31, 145, 0.772);">Contactanos</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-btn text style="color: rgba(11, 31, 145, 0.772);">Proyectos</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-btn text style="color: rgba(11, 31, 145, 0.772);">Nosotros</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
    <div>
      <v-btn text style="color: rgba(11, 31, 145, 0.772);">Cotiza</v-btn>
    </div>
    <v-divider :thickness="7" class="border-opacity-0" vertical></v-divider>
  </v-app-bar>
</template>

<script setup>
  //
</script>
