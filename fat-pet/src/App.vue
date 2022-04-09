<template>
  <div id="app">
    <NavBar />
    <div id="main">
      <SideBar />
      <DashBoard :details="details" />
    </div>
  </div>
</template>

<script>
import NavBar from "./components/NavBar";
import SideBar from "./components/SideBar";
import DashBoard from "./components/DashBoard";

export default {
  name: "App",
  components: {
    NavBar,
    SideBar,
    DashBoard,
  },
  data() {
    return {
      details: [],
    };
  },
  created() {
    this.details = [
      {
        id: 1,
        petName: "Koda",
        typeOfPet: "Dog",
        careTakers: ["Doug", "Mily"],
        snacks: 3,
        meals: [
          {
            meal: 1,
            fedBy: "Doug",
            at: "6:10am",
            status: "Ate",
          },
          {
            meal: 2,
            fedBy: "Mily",
            at: "7:00pm",
            status: "Did Not Eat",
          },
        ],
      },
      {
        id: 2,
        petName: "Teddy",
        typeOfPet: "Dog",
        careTakers: ["Maya", "Mily"],
        snacks: 1,
        meals: [
          {
            meal: 1,
            fedBy: "Maya",
            at: "6:10am",
            status: "Ate",
          },
          {
            meal: 2,
            fedBy: "Maya",
            at: "6:10am",
            status: "Ate",
          },
        ],
      },
      {
        id: 2,
        petName: "Teddy",
        typeOfPet: "Dog",
        careTakers: ["Maya", "Mily"],
        snacks: 1,
        meals: [
          {
            meal: 1,
            fedBy: "Maya",
            at: "6:10am",
            status: "Ate",
          },
          {
            meal: 2,
            fedBy: "Maya",
            at: "7:00pm",
            status: "Ate",
          },
          {
            meal: 3,
            fedBy: "Maya",
            at: "7:00pm",
            status: "Ate",
          },
        ],
      },
    ];
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
h4,
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
