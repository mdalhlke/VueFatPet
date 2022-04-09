<template>
  <div class="pet-detail">
    <h2>Name</h2>
    <div class="pet-details">
      <div class="pet-details-group">
        <h4>Meals</h4>
        <div class="pet-meals">
          <PetMeal />
          <PetMeal />
        </div>
      </div>
      <div class="pet-details-group">
        <h4>Snacks</h4>
        <h4>3</h4>
      </div>
    </div>
  </div>
</template>

<script>
import PetMeal from "./PetMeal.vue";

export default {
  name: "PetDetail",
  components: {
    PetMeal,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.pet-detail {
  padding: 1rem 2rem;
  background-color: #ffffff;
  border-radius: 10px;
}

.pet-details {
  display: flex;
  flex-direction: column;
}

.pet-details-group {
  padding: 1rem 0rem;
}

.pet-meals {
  display: flex;
  gap: 1rem;
}
</style>
