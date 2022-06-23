<template>
  <div id="app">
    <RickMorty :personajes="personajes" />
  </div>
</template>

<script>
import RickMorty from "./components/RickMorty.vue";

export default {
  name: "App",
  components: {
    RickMorty,
  },
  data() {
    return {
      personajes: [
        {
          nombre: "Rick Sanchez",
          src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        },
        {
          nombre: "Morty Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        },
        {
          nombre: "Summer Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        },
        {
          nombre: "Beth Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        },
        {
          nombre: "Jerry Smith",
          src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  background-image: url("assets/logo.png");
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
}
* {
  box-sizing: border-box;
}
</style>
