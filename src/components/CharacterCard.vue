<template>
  <div class="characterCard">
    <div class="cost">
      {{ cost }}
    </div>
    <div class="name">{{ name }}</div>
    <div class="card-img">
      <img height="100px" :src="require(`@/${cardImage}`)" alt="card image" />
    </div>
    <div class="flavortext">{{ flavortext }}</div>
    <div class="attack">{{ attack }}</div>
    <div class="health">{{ health }}</div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      name: "Lief, the Unbroken",
      attack: 2,
      health: 10,
      cost: 7,
      flavortext: "Dear Lady, I will not fail you.",
      cardImage: "assets/Lief-done.jpeg",
    };
  },
  methods: {
    getImgUrl(pic) {
      return require(pic);
    },
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

.name {
  position: absolute;
  top: 10px;
  left: 20%;
  font-size: 0.8rem;
}

.flavortext {
  font-size: 0.6rem;
  position: absolute;
  bottom: 30px;
  left: 2px;
  padding: 5px;
  text-align: center;
}

.card-img {
  height: 200px;
  width: 200px;
  position: absolute;
  top: 35px;
  left: 26px;
}
</style>
