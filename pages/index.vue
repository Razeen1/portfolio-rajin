<template>
  <v-container class="pa-0" fluid>
    <div style="position: relative">
      <v-img class="bannerImage" cover height="100vh" src="/banner3.jpg">
        <v-card class="pa-6  position-relative banner h-100 d-flex" color="transparent" flat rounded="0">
          <div class="d-flex flex-column" style="position: absolute;top:20%;right:2%">
            <v-icon class="mt-12" color="#2E382E">mdi-facebook</v-icon>
            <v-icon class="mt-12" color="#2E382E">mdi-instagram</v-icon>
            <v-icon class="mt-12" color="#2E382E">mdi-linkedin</v-icon>
          </div>
          <v-row align="end" class="" style="pointer-events: none;">
            <v-col class="text-left" cols="12">
              <span
                  style="font-size:70px;font-weight:100!important;line-height:70px;color: #A1BA89;text-transform: uppercase;">Hi! I'm
                Rajin <span
                    class="font-weight-thin" style="color:#382633"> Bhuju</span>
              </span>
              <span class=" pl-6 text-grey">Graphics Designer | Front-end Developer
              </span>
            </v-col>
          </v-row>
        </v-card>
      </v-img>

    </div>
<!--    <v-img src="/banner4.jpg" height="450" cover>-->
    <v-card class="aboutMe" color="transparent" flat height="650">
      <v-card-text>
        <div class="abtImage1">
          <v-img src="/img1.jpg"></v-img>
        </div>
        <div class="abtImage2">
          <v-img src="/img2.jpg"></v-img>
        </div>
        <div class="text-h2"
             style="writing-mode: vertical-lr;text-orientation: revert;color:#B98389;position: absolute;right:12%;top:17%">
          About Me
        </div>
        <div class="text-body text-justify" style="width: 500px;position: absolute;right:15%;top:25%">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus mauris leo, vestibulum a tristique id,
            rhoncus sed ligula. Nunc efficitur accumsan erat ac volutpat. Vestibulum malesuada a erat id euismod. Nunc
            consectetur velit a blandit ultricies. Morbi maximus urna a libero aliquam, at laoreet metus euismod.
            Phasellus laoreet sodales porta. Quisque sollicitudin urna eget ex interdum posuere.</p>
          <p>Aenean aliquam mi vel justo venenatis gravida. Nam metus eros, aliquet sed libero at, scelerisque malesuada
            ipsum. Morbi quis dolor nec leo blandit posuere. In blandit convallis dui, quis posuere justo ultricies
            sed. </p>
        </div>
      </v-card-text>
    </v-card>
    <v-card class="mx-6 pa-6" flat>
      <v-card-text>
        <span class="text-h2 font-weight-bold projectText pb-2">Projects</span>
        <v-row>
          <v-col cols="3">
            <v-card flat height="300px" image="/img1.jpg" rounded="0" subtitle="HEllow this is world"
                    title="Hello World"></v-card>
          </v-col><v-col cols="3">
            <v-card flat height="300px" image="/img1.jpg" rounded="0" subtitle="HEllow this is world"
                    title="Hello World"></v-card>
          </v-col><v-col cols="3">
            <v-card flat height="300px" image="/img1.jpg" rounded="0" subtitle="HEllow this is world"
                    title="Hello World"></v-card>
          </v-col>

        </v-row>

      </v-card-text>
    </v-card>
  </v-container>
</template>
<script setup>
import VanillaTilt from 'vanilla-tilt'
import {onMounted, ref} from 'vue'

const element = ref(null)

onMounted(() => {
  VanillaTilt.init(element.value, {max: 40, speed: 200})
})
</script>

<style>
.card1 {
  height: 400px;
  background: radial-gradient(circle at 100px 100px, #D37F7F, #3b1e1e);
  //background-color: #D37F7F;
  position: absolute;
  width: 400px;
  bottom: 50px;
  left: 300px;
  border-radius: 20000px;
  z-index: -2;
}

.textHero {
  position: absolute;
  width: 300px;
  right: 200px;
  top: 50px;
}

.card2 {
  height: 200px;
  background-color: #051010;
  position: absolute;
  width: 150px;
  top: 40px;
  right: 170px;
  opacity: 0.4;
  z-index: -2;
}

.welcome-text {
  height: 40px;
  overflow: hidden;
}

.line {
  text-transform: uppercase;
  font-size: 40px;
  line-height: 50px;
}

.line:first-child {
  animation: a 10s infinite;
}

@keyframes a {
  0% {
    margin-top: 0px;
  }
  16% {
    margin-top: -60px;
  }
  33% {
    margin-top: -120px;
  }
  50% {
    margin-top: -180px;
  }
  66% {
    margin-top: -120px;
  }
  82% {
    margin-top: -60px;
  }
  100% {
    margin-top: 0px;
  }
}

.shape1 {
  width: 90px;
  height: 90px;
  background-color: rgba(129, 133, 113, 0.11);
  position: absolute;
  top: 2%;
  right: 20%;
  animation-name: floating2;
  animation-duration: 10s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  border-radius: 38% 62% 67% 33% / 26% 30% 70% 74%;
}

.shape2 {
  width: 400px;
  height: 400px;
  background: rgb(40, 149, 245);
  background: linear-gradient(111deg, rgba(40, 149, 245, 0.1) 0%, rgba(40, 177, 245, 0.4) 50%, rgba(145, 40, 245, 0.1) 100%);
  position: absolute;
  top: 10%;
  left: 20%;
  z-index: -1;
  animation-name: floating2;
  animation-duration: 9s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  border-radius: 38% 62% 67% 33% / 40% 49% 51% 60%;
}

.shape3 {
  width: 30px;
  height: 30px;
  background-color: rgba(255, 255, 255, 0.09);
  position: absolute;
  top: 5%;
  left: 80%;
  animation-name: floating2;
  animation-duration: 9s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  animation-delay: 4s;
  border-radius: 38% 62% 67% 33% / 26% 30% 70% 74%;
}

@keyframes floating {
  0% {
    transform: translate(0, 0px);
  }
  50% {
    transform: translate(-10px, 5px);
  }

  100% {
    transform: translate(-0px, -0px);
  }
}


@keyframes floating2 {
  0% {
    transform: translate(0, 0px);
  }
  50% {
    transform: translate(2px, 20px);
  }

  100% {
    transform: translate(-0px, -0px);
  }
}

.banner {
  background: rgb(71, 147, 175) !important;
  background: linear-gradient(180deg, rgba(71, 147, 175, 0.9) 0%, rgba(71, 147, 175, 0) 63%) !important;
}

.bannerImage {
  position: absolute;
  top: 0;
}

.abtImage1 {
  width: 250px;
  position: absolute;
  top: 20%;
  left: 20%;
}

.abtImage2 {
  position: absolute;
  width: 250px;
  top: 30%;
  left: 5%;

}

.projectSection {
  background: rgba(185, 131, 137) !important;
  background: linear-gradient(180deg, rgba(71, 147, 175, 0) 0%, rgba(185, 131, 137, 0.8) 100%) !important;
}


</style>