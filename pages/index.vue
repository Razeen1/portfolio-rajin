<template>
  <v-container class="pa-0" fluid>
    <v-card class="pt-6 position-relative" color="#0E2F2F" height="550" rounded="0">
      <div class="card1"></div>
      <v-row align="center" class="ma-6 pa-6 ">
        <v-col cols="8">
          <div class="text-h2 font-weight-thin">Hey!!</div>
          <div class="text-h1 font-weight-black">welcome.</div>
          <div class="text-h5 pt-6 font-weight-medium">I'm <strong>Rajin</strong>. <span class="text-h6">you are viewing my portfolio.</span></div>
        </v-col>
        <v-col class="" cols="2">
          <div class="text-h4 text-white font-weight-black mb-3">why so creative?</div>
          <div class="text-body-1 text-white font-weight-thin"> Lorem ipsum dolor sit amet, consectetur
            adipiscing elit.
            Sed molestie sapien sit amet nibh vestibulum, a tristique elit pulvinar. Cras luctus odio arcu, eu imperdiet
          </div>
        </v-col>
      </v-row>
    </v-card>
  </v-container>
</template>
<script lang="ts" setup>
</script>

<style>
.card1 {
  height: 400px;
  background-color: #051010;
  position: absolute;
  width: 500px;
  bottom: 50px;
  left: 300px;
  z-index: -2;
}
</style>