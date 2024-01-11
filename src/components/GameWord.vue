<template>
  <div class="word">
    <span v-for="(letter, index) in word" :key="index" class="letter" />
  </div>
</template>

<script setup lang="ts">


interface Props {
  word: string;
}
defineProps<Props>();
</script>
