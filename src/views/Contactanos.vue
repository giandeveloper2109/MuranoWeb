<template>
        

    <h1 class="text-center"  style="color:  rgb(10, 10, 50);">Contactanos</h1>

            
        

        
    <div>   
    <v-row>
        
        <v-col>
            
            <ContatenosMediosDeComunicacion/>
        </v-col>
        
        <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
        
        <v-col>
            <ContactenosFormulario/>
        </v-col>
        
    </v-row>
    </div> 
</template>
  
<script setup>
    import ContactenosFormulario from '@/components/VistaContactenos/ContactenosFormulario.vue';
    import ContatenosMediosDeComunicacion from '@/components/VistaContactenos/ContatenosMediosDeComunicacion.vue';
</script>

<style>

</style>
