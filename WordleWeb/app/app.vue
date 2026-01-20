<template>
  <v-container>
    <v-btn variable="flat" color="primary">Hello</v-btn>
  </v-container>
</template>
<script setup lang="ts">
  const guesses: Ref<Array<Array<Letter>>> = ref([]);
  const targetWord = ref("");
  const guess = ref("");

  function submit() {

  }
  class Letter {
    character: string;
    state: LetterState;
    constructor(character: string, state: LetterState) {
      this.character = character;
      this.state = state;
    }

  }
  enum LetterState {
    Correct,
    Misplaced,
    Wrong,
  }
</script>