<template>
  <div>
    <v-card class="mx-auto" max-width="344">
      <v-img :src="personaje.imagen" height="200px"></v-img>
      <v-card-title>
        {{ personaje.nombre }}
      </v-card-title>
      <v-card-actions>
        <v-btn color="orange lighten-2" text>
          Explore
        </v-btn>
      </v-card-actions>
    </v-card>
  </div>
</template>
<script>
export default {
  props: {
    personaje: Object
  }
};
</script>
<style></style>
