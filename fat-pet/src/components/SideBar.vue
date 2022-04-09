<template>
  <div id="side-bar">
    <h2 style="padding-bottom: 1rem">Actions</h2>
    <div id="items">
      <div id="action-items">
        <div class="item-group">
          <p @click="fedPet()" class="action-btn">Fed my pet</p>
          <p @click="excersiedPet()" class="action-btn">Excersied</p>
        </div>
        <div class="item-group">
          <p @click="addPet()" class="action-btn">Add a Pet</p>
          <p @click="addCareTaker()" class="action-btn">Add a Care Taker</p>
        </div>
        <div>
          <p @click="openCalendar()" class="action-btn">Calendar View</p>
        </div>
      </div>
      <div>
        <p @click="openAbout()" class="action-btn">About</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SideBar",
  methods: {
    fedPet() {
      alert("YOU FED YOUR PET");
    },
    excersiedPet() {
      alert("YOU WALKED YOUR PET");
    },
    addPet() {
      alert("YOU ADDED A NEW PET");
    },
    addCareTaker() {
      alert("YOU ADDED A NEW CARE TAKER");
    },
    openCalendar() {
      alert("OPEN CAL");
    },
    openAbout() {
      alert("OPEN ABOUT");
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#side-bar {
  position: relative;
  display: flex;
  flex-direction: column;
  padding: 1rem 2rem;
  background-color: #ffba33;
  width: 20%;
}

#items {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100vh;
}

#action-items {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.item-group {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.action-btn {
  cursor: pointer;
}
</style>
