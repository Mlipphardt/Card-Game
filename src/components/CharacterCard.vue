<template>
  <div class="characterCard">
    <div class="cost">
      {{ cost }}
    </div>
    <div class="name"></div>
    <div class="attack">{{ attack }}</div>
    <div class="health">{{ health }}</div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      attack: 2,
      health: 1,
      cost: 1,
    };
  },
};
</script>

<style>
.characterCard {
  position: relative;
  height: 205px;
  width: 137px;
  background-color: red;
}

.cost .attack .health {
  background-color: white;
}

.cost {
  position: absolute;
  top: 10px;
  left: 10px;
}

.attack {
  position: absolute;
  bottom: 5px;
  left: 10px;
}

.health {
  position: absolute;
  bottom: 5px;
  right: 10px;
}
</style>
