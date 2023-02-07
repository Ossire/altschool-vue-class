

<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script>
import { ref, reactive } from "@vue/reactivity";
import colorEngine from "./composables/colorengine.js"

export default {
  
  setup() {
    const {colors, message, matchColor} = colorEngine()

     return { colors, message, matchColor }
  },

 
};




</script>

<style></style>
Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
altschool-class-of-vue/ColorPickerGame.vue at master · iykeevans/altschool-class-of-vue · GitHub