<template>
  <div class="meal">
    <p style="font-weight: 500">1st</p>
    <div>
      <div class="meal-details">
        <div><p>Fed By:</p></div>
        <div><p style="color: #3378ff">Doug</p></div>
      </div>
      <div class="meal-details">
        <div><p>At:</p></div>
        <div><p>6:10am</p></div>
      </div>
      <div class="meal-details">
        <div><p>Status:</p></div>
        <div><p>Ate</p></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PetMeal",
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
  box-shadow: 0px 0px 5px #c4c4c4;
  border-radius: 10px;
  padding: 1rem;
}

.meal-details {
  display: flex;
}
</style>
