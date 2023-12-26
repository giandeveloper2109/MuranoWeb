<template>

 
        <v-sheet>
            <v-img src="@/assets/logoMurano.png" max-height="100"></v-img>

                
            <v-row>
                <v-col class="d-flex align-center justify-center">
                    <v-card  @click="redirectToPhone"
                        height="70"
                        width="250"
                        style="background-color: #000744;color: rgb(255, 255, 255);;"
                        class="d-flex align-center justify-center"
                        
                    >
                        <v-row>
                            <v-col>
                                <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
                                <v-icon class="icon-size" icon="mdi-phone"></v-icon>
                                <v-divider :thickness="10" class="border-opacity-0" vertical></v-divider>
                                <span>Telefono (074) 600 993</span>
                            </v-col>

                        </v-row>
                    </v-card>
                    
                </v-col>


                <v-col class="d-flex align-center justify-center">
                    <v-card  @click="redirectToPhone"
                        height="70"
                        width="250"
                        style="background-color: #000744;color: rgb(255, 255, 255);;"
                        class="d-flex align-center justify-center"
                        
                    >
                        <v-row>
                            <v-col>
                                <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
                                <v-icon class="icon-size" style="color: rgb(38, 141, 28);" icon="mdi mdi-whatsapp"></v-icon>
                                <v-divider :thickness="10" class="border-opacity-0" vertical></v-divider>
                                <span>+51 982 010 512</span>
                            </v-col>

                        </v-row>
                    </v-card>
                    
                </v-col>


                <v-col class="d-flex align-center justify-center">
                    <v-card  
                        height="70"
                        width="250"
                        style="background-color: #000744;color: rgb(255, 255, 255);;"
                        class="d-flex align-center justify-center"
                        
                    >
                        <v-row>
                            <v-col>
                                <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
                                <v-icon icon="mdi mdi-map-marker"></v-icon>
                                <v-divider :thickness="10" class="border-opacity-0" vertical></v-divider>
                                <span>Calle 7 de Enero #660 Chiclayo</span>
                            </v-col>

                        </v-row>
                    </v-card>
                    
                </v-col>


                <v-col class="d-flex align-center justify-center">
                    <v-card  @click="redirectMail"
                        height="70"
                        width="250"
                        style="background-color: #000744;color: rgb(255, 255, 255);;"
                        class="d-flex align-center justify-center"
                        
                    >
                        <v-row>
                            <v-col>
                                <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
                                <v-icon icon="mdi mdi-email"></v-icon>
                                <v-divider :thickness="10" class="border-opacity-0" vertical></v-divider>
                                <span>info@muranoin.com</span>
                            </v-col>

                        </v-row>
                    </v-card>
                    
                </v-col>

            </v-row>


            
        </v-sheet>


</template>
<script>
export default {
  methods: {
    redirectToWhatsApp() {
      // Reemplaza '123456789' con el número de teléfono al que deseas redirigir en formato internacional.
      const phoneNumber = '51982010512';

      // Abre la ventana de WhatsApp con el número de teléfono.
      window.location.href = `https://wa.me/${phoneNumber}`;
    },
    redirectToPhone() {
        window.location.href = `tel:074600993`;
    },
    redirectMail () {
  window.location.href = `mailto:info@muranoin.com`;
}
    
  }
}
</script>
<style>
  .icon-size {
    font-size: 40px; 
  }
</style>