<template>
  <div class="pet-detail">
    <h2>{{ detail.petName }}</h2>
    <div class="pet-details">
      <div class="pet-details-group">
        <h4 style="padding-bottom: 1rem">Meals</h4>
        <div class="pet-meals">
          <div :key="meal.meal" v-for="meal in detail.meals">
            <PetMeal :meal="meal" />
          </div>
        </div>
      </div>
      <div class="pet-details-group">
        <h4>Snacks</h4>
        <div class="pet-snacks">
          <b-icon icon="dash-circle" font-scale="1" style="color: #3378ff">
          </b-icon>
          <h4>{{ detail.snacks }}</h4>
          <b-icon icon="plus-circle" font-scale="1" style="color: #3378ff">
          </b-icon>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import PetMeal from "./PetMeal";

export default {
  name: "PetDetail",
  components: {
    PetMeal,
  },
  props: {
    detail: Object,
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
  padding-top: 1rem;
}

.pet-meals {
  display: flex;
  gap: 1rem;
}

.pet-snacks {
  display: flex;
  align-items: center;
  gap: 1rem;
}
</style>
