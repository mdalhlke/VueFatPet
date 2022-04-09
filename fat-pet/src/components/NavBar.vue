<template>
  <div id="nav-bar">
    <h1>Fat Pet</h1>
    <b-icon icon="person-circle" font-scale="3"></b-icon>
  </div>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Fredoka+One");

h1 {
  font-family: "Fredoka One", sans-serif;
}

#nav-bar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 2rem;
  background-color: #ffffff;
  height: 100px;
}
</style>
