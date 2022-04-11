<template>
  <v-footer dark padless>
    <v-card flat tile class="black white--text py-12 px-5" width="100%">
      <v-row>
        <v-col cols="12" xs="12" sm="6" md="4" class="pa-16">
          <v-toolbar color="transparent" flat>
            <v-badge color="#d5f0db" dot>
              <v-img src="1.png" contain width="30"></v-img>
            </v-badge>
            <v-toolbar-title class="ml-4">
              <span class="green--text">e</span><strong>Grocery</strong>
            </v-toolbar-title>
          </v-toolbar>
          <v-card-text class="pt-0">
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-1 white--text"
              icon
              fab
              outlined
              small
            >
              <v-icon size="20px">
                {{ icon }}
              </v-icon>
            </v-btn>
          </v-card-text>
        </v-col>
        <v-col cols="12" xs="12" sm="6" md="2">
          <v-card-text class="white--text pt-0">
            <h3>Acerca de</h3>
          </v-card-text>
          <v-card-text class="grey--text"> Cómo Funciona</v-card-text>
          <v-card-text class="grey--text mt-n4"> Nuestros Programas</v-card-text>
          <v-card-text class="grey--text mt-n4"> Promociones</v-card-text>
          <v-card-text class="grey--text mt-n4"> Referir a un amigo</v-card-text>
        </v-col>
        <v-col cols="12" xs="12" sm="6" md="2">
          <v-card-text class="white--text pt-0">
            <h3>Delivery</h3>
          </v-card-text>
          <v-card-text class="grey--text"> Costo del Delivery</v-card-text>
          <v-card-text class="grey--text mt-n4"> Métodos de Pago</v-card-text>
          <v-card-text class="grey--text mt-n4"> Estado del Delivery</v-card-text>
          <v-card-text class="grey--text mt-n4"> Retornos</v-card-text>
        </v-col>
        <v-col cols="12" xs="12" sm="6" md="2">
          <v-card-text class="white--text pt-0">
            <h3>Contacto</h3>
          </v-card-text>
          <v-card-text class="grey--text"> Yenifer Rosana</v-card-text>
          <v-card-text class="grey--text mt-n4"> Mérida, Venezuela</v-card-text>
          <v-card-text class="grey--text mt-n4"> @yeniferrosana</v-card-text>
          <v-card-text class="grey--text mt-n4"> B81234567</v-card-text>
        </v-col>
      </v-row>
    </v-card>
  </v-footer>
</template>
<script>
export default {
  data: () => ({
    icons: [
      "fab fa-apple",
      "fab fa-google-plus-g",
      "fab fa-twitter",
      "fab fa-facebook-f"
    ]
  }),
}
</script>