<template>
  <v-container>
    <v-row>
      <v-col class="mx-auto">
        <CharacterCard />
      </v-col>
    </v-row>
    <v-row>
      <PlayerDashboard>
        <CharacterCard />
      </PlayerDashboard>
    </v-row>
  </v-container>
</template>

<script>
import CharacterCard from "../components/CharacterCard";
import PlayerDashboard from "../components/PlayerDashboard";

export default {
  name: "index",
  components: {
    CharacterCard,
    PlayerDashboard,
  },
  data: () => {},
};
</script>

<style></style>
