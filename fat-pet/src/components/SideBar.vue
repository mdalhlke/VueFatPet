<template>
  <div id="side-bar">
    <h2 style="padding-bottom: 1rem">Actions</h2>
    <div id="items">
      <div id="action-items">
        <div class="item-group">
          <p>Fed my pet</p>
          <p>Excersied</p>
        </div>
        <div class="item-group">
          <p>Add a Pet</p>
          <p>Add a Care Taker</p>
        </div>
        <div>
          <p>Calendar View</p>
        </div>
      </div>
      <div>
        <p>About</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SideBar",
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
</style>
