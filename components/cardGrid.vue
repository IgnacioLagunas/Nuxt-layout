<template>
  <div>
    <v-container class="mt-6">
      <template>
        <v-row>
          <v-col v-for="(personaje, index) in personajes" :key="index" md="4">
            <Card :personaje="personaje"></Card>
          </v-col>
        </v-row>
      </template>
    </v-container>
  </div>
</template>
<script>
import card from "@/components/card.vue";
export default {
  components: {
    card
  },
  data: () => ({
    personajes: [
      {
        id: 1,
        nombre: "Morty",
        imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg"
      },
      {
        id: 2,
        nombre: "Rick",
        imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg"
      },
      {
        id: 3,
        nombre: "Summer",
        imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg"
      },
      {
        id: 4,
        nombre: "Beth",
        imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg"
      },
      {
        id: 5,
        nombre: "Jerry",
        imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg"
      }
    ]
  })
};
</script>
<style></style>
