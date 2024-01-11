<template>
  <game-header />
  <div class="game-container">
    <game-figure />
    <game-wrong-letters />
    <game-word :word="word" />
  </div>
  <game-popup />
  <game-notification />
</template>

<script setup lang="ts">
import GameHeader from "@/components/GameHeader.vue";
import GameFigure from "@/components/GameFigure.vue";
import GameWrongLetters from "@/components/GameWrongLetters.vue";
import GameWord from "@/components/GameWord.vue";
import GamePopup from "@/components/GamePopup.vue";
import GameNotification from "@/components/GameNotification.vue";

import { ref } from "vue";

const word = ref("василий");
</script>

<style scoped></style>
