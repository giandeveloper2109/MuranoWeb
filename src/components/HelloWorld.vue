<template>
  <v-row>
    <v-col>
      <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <v-img height="300" src="@/assets/construccion.png" />

      <div class="text-body-2 font-weight-light mb-n1">Bienvenido a Murano</div>

      <h1 class="text-h2 font-weight-bold">Regresaremos pronto</h1>

      <div class="py-14" />

    </v-responsive>
      </v-container>
    </v-col>
    
    <v-col>
      <v-container >
    <v-responsive class="align-center text-center fill-height">
      <ContatenosMediosDeComunicacion/>
    </v-responsive>
  </v-container>
    </v-col>
  </v-row>

</template>

<script setup>
  import ContatenosMediosDeComunicacion from './VistaContactenos/ContatenosMediosDeComunicacion.vue';
</script>
