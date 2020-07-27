<template>
  <v-container>
    <v-row>
      <v-col cols="2">Aw snap </v-col>
      <v-col cols="10">
        <v-row>
          <slot></slot>
          <slot></slot>
          <slot></slot>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style></style>
