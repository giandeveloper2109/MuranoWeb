<template>
    <div>
        
        <v-sheet>
            <v-img src="@/assets/logoMurano.png" max-height="100"></v-img>
            <div>
            <v-row>
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
                                <v-icon icon="mdi-phone"></v-icon>
                                <v-divider :thickness="10" class="border-opacity-0" vertical></v-divider>
                                <span>Telefono (074) 600 993</span>
                            </v-col>

                        </v-row>
                    </v-card>
                    
                </v-col>
                <v-col>
                    <v-card @click="redirectToWhatsApp"
                    height="70"
                        width="250"
                        style="background-color: #000744;color: rgb(255, 255, 255);;"
                        class="d-flex align-center justify-center" 
                    >
                    <v-row>
                            <v-col>
                                <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
                                <v-icon  icon="mdi mdi-whatsapp" color="green"></v-icon>
                                <v-divider :thickness="10" class="border-opacity-0" vertical></v-divider>
                                <span class="align-center justify-center"> +51 982 010 512</span>
                            </v-col>

                        </v-row>
                    </v-card>
                </v-col>
            </v-row>
            </div>
            <div>
            <v-row>
                <v-col>
                    <v-card class="d-flex align-center justify-center" ></v-card>
                </v-col>
                <v-col>
                    <v-card class="d-flex align-center justify-center" ></v-card>
                </v-col>
            </v-row>
        </div>

            
        </v-sheet>
    </div>
</template>
<script>
export default {
  methods: {
    redirectToWhatsApp() {
      // Reemplaza '123456789' con el número de teléfono al que deseas redirigir en formato internacional.
      const phoneNumber = '51982010512';

      // Abre la ventana de WhatsApp con el número de teléfono.
      window.location.href = `https://wa.me/${phoneNumber}`;
    }
  }
}
</script>