<template>
  <div id="dashboard">
    <div id="title-contents">
      <div>
        <h2>Dashboard</h2>
      </div>
      <div>
        <p>April 20, 2022</p>
      </div>
    </div>
    <div id="pet-detail-blocks">
      <PetDetail />
      <PetDetail />
    </div>
  </div>
</template>

<script>
import PetDetail from "./PetDetail.vue";

export default {
  name: "DashBoard",
  components: {
    PetDetail,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#dashboard {
  padding: 1rem 2rem;
  background-color: #f3f3f3;
  width: 100%;
  overflow-y: scroll;
}

#title-contents {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f3f3f3;
  padding-bottom: 1rem;
}

#pet-detail-blocks {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
</style>
