<template>
  <v-app>
    <v-app-bar absolute flat color="#0E2F2F">
      <v-app-bar-title class="font-weight-bold pa-6">logo.</v-app-bar-title>
      <v-spacer></v-spacer>
      <v-btn>Apple</v-btn>
      <v-btn>Apple</v-btn>
      <v-btn>Apple</v-btn>
      <v-spacer></v-spacer>
    </v-app-bar>
    <v-main>
      <slot/>
    </v-main>
  </v-app>
</template>
<script lang="ts" setup>
</script>