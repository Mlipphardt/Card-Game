<template>
  <v-container>
    <v-row>
      <v-col class="mx-auto">
        <CharacterCard />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import CharacterCard from "../components/CharacterCard";
export default {
  name: "index",
  components: {
    CharacterCard,
  },
  data: () => {},
};
</script>

<style></style>
