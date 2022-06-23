<template>
  <div>
    <ul>
      <li v-for="{ nombre, src } in personajes">
        <img :src="src" class="avatar" />
        <p>{{ nombre }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "RickMorty",
  props: {
    personajes: [],
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: flex;
  justify-content: start;
  align-items: center;
  gap: 30px;
  padding-top: 30px;
  margin: 20px 20px;
  color: white;
  font-size: 20px;
}

.avatar {
  border: 1px solid #ddd;
  border-radius: 50%;
  padding: 5px;
  width: 120px;
}
</style>
