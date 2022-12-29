<script setup lang="ts">
import FancyButton from "@/components/FancyButton.vue";
import { mdiFaceWoman, mdiArrowBottomRightBoldOutline } from "@mdi/js";
</script>

<template>
  <v-container>
    <v-row>
      <v-col
        ><FancyButton
          ><v-icon :icon="mdiFaceWoman" />Hug Me
          <template v-slot:tail> Tail </template>
        </FancyButton></v-col
      ><v-col
        ><FancyButton
          ><v-icon :icon="mdiArrowBottomRightBoldOutline" />Click Me
          <template v-slot:tail> My Tail </template>
        </FancyButton></v-col
      >
    </v-row>
  </v-container>
</template>
