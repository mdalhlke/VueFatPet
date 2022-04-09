<template>
  <div class="meal">
    <p style="font-weight: 500">{{ meal.meal }}</p>
    <div>
      <div class="meal-details">
        <div><p>Fed By:&nbsp;</p></div>
        <div>
          <p style="color: #3378ff">{{ meal.fedBy }}</p>
        </div>
      </div>
      <div class="meal-details">
        <div><p>At:&nbsp;</p></div>
        <div>
          <p>{{ meal.at }}</p>
        </div>
      </div>
      <div class="meal-details">
        <div><p>Status:&nbsp;</p></div>
        <div>
          <p>{{ meal.status }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PetMeal",
  props: {
    meal: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.meal {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 15rem;
  background-color: #ffffff;
  box-shadow: 0px 0px 5px #d9d9d9;
  border-radius: 10px;
  padding: 1rem;
}

.meal-details {
  display: flex;
}
</style>
