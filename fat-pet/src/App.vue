<template>
  <div id="app">
    <NavBar />
    <div id="main">
      <SideBar />
      <DashBoard />
    </div>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import SideBar from "./components/SideBar.vue";
import DashBoard from "./components/DashBoard.vue";

export default {
  name: "App",
  components: {
    NavBar,
    SideBar,
    DashBoard,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Rubik:wght@400;500&display=swap");

p {
  font-weight: 400;
  font-size: 20px;
}

h1,
h2,
h3,
p {
  margin: 0 !important;
}

#app {
  font-family: "Rubik", sans-serif;
}

#main {
  display: flex;
  height: calc(100vh - 100px);
}
</style>
