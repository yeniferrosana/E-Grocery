<template>
  <v-item-group mandatory class="mt-n1">
    <v-container>
      <v-row justify="center" class="space">
        <v-col 
          cols="12" xs="12" sm="4" md="2"
          v-for="(category, i) in categories"
          :key="i"
        >
          <v-item v-slot="{ active, toggle }">
            <v-card 
              :color="active ? '#d5f0db': 'white'"
              :style="active ? 'border: 3px solid green;'  : 'border: 1px solid white;'"
              class="d-flex align-center rounded-lg mx-2"
              dark
              height="180"
              flat
              @click="toggle"
            >
              <v-row>
                <v-col cols="12" sm="12">
                  <v-list-item three-line class="text-center">
                    <v-list-item-content>
                      <div align="center" justify="center">
                        <v-img :src="category.img" max-height="80" max-width="80" contain></v-img>
                      </div>
                      <v-list-item-subtitle
                        :class="active ? 'green--text': 'black--text'"
                        class="caption mt-4"
                      >
                        {{ category.title}}
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>
            </v-card>
          </v-item>

        </v-col>
      </v-row>
    </v-container>
  </v-item-group>
</template>
<script>

export default {
  data: () => ({
    categories: [
      { img: "01.png", title: "Carnes y Pescados" },
      { img: "02.png", title: "Vegetales" },
      { img: "3.png", title: "Medicina" },
      { img: "4.png", title: "Bébes" },
      { img: "5.png", title: "Oficina" },
      { img: "6.png", title: "Cosméticos" }
    ]
  })
}
</script>

<style scoped>

</style>
