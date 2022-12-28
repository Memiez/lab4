<script setup lang="ts">
import { ref } from "vue";
const props = defineProps<{
  name: string;
  img: string;
  rating: number;
}>();

const count = ref(props.rating);
function inc() {
  count.value++;
}
function dec() {
  count.value--;
}
</script>

<template>
  <v-card class="mx-auto" max-width="344" variant="outlined">
    <v-img :src="props.img" height="200px"></v-img>
    <v-card-item>
      <div class="text-center">
        <div class="text-overline mb-1">{{ props.name }}</div>
        <div class="text-h6 mb-1">Score: {{ count }}</div>
      </div>
    </v-card-item>

    <v-card-actions class="justify-center">
      <v-btn variant="flat" color="#F67280" @click="dec()"> - </v-btn>
      <v-btn variant="flat" color="#1E90FF" @click="inc()"> + </v-btn>
    </v-card-actions>
  </v-card>
</template>
