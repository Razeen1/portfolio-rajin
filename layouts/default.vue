<template>
  <v-app>
    <v-app-bar flat absolute color="transparent" class="text-white">
      <v-app-bar-title class="font-weight-bold pa-6">logo.</v-app-bar-title>
      <v-spacer></v-spacer>
      <v-btn>Apple</v-btn>
      <v-btn>Apple</v-btn>
      <v-btn>Apple</v-btn>
      <v-spacer></v-spacer>
    </v-app-bar>
    <v-main class="pt-0">
      <slot/>
    </v-main>
  </v-app>
</template>
<script lang="ts" setup>
</script>