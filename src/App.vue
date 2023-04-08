<template>
  <div class="container">
    <div class="row my-5">
      <div class="col-md-8 offset-2">
        <div v-if="active">
          <h2 class="mb-3">Log in</h2>
          <button class="btn btn-success" @click="active = false">login</button>
        </div>
        <div v-else-if="!active">
          <h2 class="mb-3">Welcome</h2>
          <button class="btn btn-success" @click="active = true">logout</button>
        </div>
      </div>
    </div>
    <div class="row my-5">
      <div class="col-md-8 offset-2">
        <div class="wrapper">
          <HeaderApp :open="open" :close="close" />
          <div class="wrapper__middle">
            <NavbarApp :open="open" :close="close" />
            <div class="wrapper__section">
              <SectionApp />
              <SectionApp />
              <SectionApp />
            </div>
          </div>
          <FooterApp :open="open" :close="close" />
        </div>
      </div>
    </div>
    <div class="row my-5">
      <div class="col-md-8 offset-2">
        <div class="wrapper__2">
          <Gorilla :gorilla_info="gorilla_info"/>
          <Lion :lion_info="lion_info"/>
          <Zebra :zebra_info="zebra_info"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

import { ref } from 'vue';
import HeaderApp from './components/header/HeaderApp.vue';
import NavbarApp from './components/navbar/NavbarApp.vue';
import SectionApp from './components/section/SectionApp.vue';
import FooterApp from "./components/footer/FooterApp.vue"
import Gorilla from "./components/gorilla/Gorilla.vue"
import Lion from "./components/lion/Lion.vue"
import Zebra from "./components/zebra/Zebra.vue"

const active = ref(true)
const open = ref("<")
const close = ref(">")
const gorilla_info = ref({
  name: "Gorilla",
  last_name: "Gorilla beringei",
  weight: "205kg",
  foods: "plants, insects"
})

const lion_info = ref({
  name: "Lion",
  last_name: "Panthera leo",
  weight: "140kg",
  foods: "meat"
})

const zebra_info = ref({
  name: "Zebra",
  last_name: "Equus quaga",
  weight: "322kg",
  foods: "plants"
})

</script>

<style scoped>
.wrapper {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.wrapper__middle {
  display: flex;
  gap: 10px;
}

.wrapper__section {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.wrapper__2{
  display: flex;
  justify-content: space-between;
}

</style>