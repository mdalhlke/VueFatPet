<template>
  <div id="dashboard">
    <div id="title-contents">
      <div>
        <h2>Dashboard</h2>
      </div>
      <div>
        <p>{{ currentDate() }}</p>
      </div>
    </div>
    <div id="pet-detail-blocks">
      <div :key="detail.id" v-for="detail in details">
        <PetDetail :detail="detail" />
      </div>
    </div>
  </div>
</template>

<script>
import PetDetail from "./PetDetail";

export default {
  name: "DashBoard",
  components: {
    PetDetail,
  },
  props: {
    details: Array,
  },
  methods: {
    currentDate() {
      const current = new Date();
      const options = {
        weekday: "long",
        year: "numeric",
        month: "long",
        day: "numeric",
      };
      return current.toLocaleString("en-US", options);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#dashboard {
  background-color: #f3f3f3;
  width: 100%;
  overflow-y: scroll;
}

#title-contents {
  position: sticky;
  top: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f3f3f3;
  padding: 1rem 2rem;
}

#pet-detail-blocks {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  margin: 1rem 2rem;
}
</style>
