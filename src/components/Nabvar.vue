<template>
  <v-app-bar app color="white" flat>
    <v-badge color="#D5F0DB" dot>
      <v-img src="1.png" contain width="30"></v-img>
    </v-badge>
    <v-toolbar-title class="ml-4">
      <span class="green--text">e</span><strong>Grocery</strong>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-badge color="#ff6d59" overlap content="2" class="mr-2 mt-1">
      <v-avatar color="fff0ee" size="40">
        <v-icon x-small color="#ff6d59">far fa-heart</v-icon>
      </v-avatar>
    </v-badge>
    <v-badge color="#41ab55" overlap content="3" class="mr-2 mt-1">
      <v-avatar color="#ECF7EE" size="40">
        <v-icon x-small color="#41ab55">fas fa-shopping-cart</v-icon>
      </v-avatar>
    </v-badge>
    <span class="grey--text d-none d-sm-flex">Hola, <strong> Rosana</strong></span>
    <v-avatar size="30" class="ml-2">
      <v-img src="avatar.jpg"></v-img>
    </v-avatar>
    <v-btn icon dark>
      <v-icon x-small color="#878a94">fas fa-chevron-down</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>

export default {

}
</script>
<style scoped>
.v-toolbar__title{
  font-size: 1rem !important;
}
</style>