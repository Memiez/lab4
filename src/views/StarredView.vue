<script setup lang="ts">
import FrameworkPop from "@/components/FrameworkPop.vue";
const frameList = [
  {
    name: "VueJS",
    img: "https://img.icons8.com/color/512/vue-js.png",
    rating: 10,
  },
  {
    name: "AngularJS",
    img: "https://img.icons8.com/fluency/512/angularjs.png",
    rating: 19,
  },
  {
    name: "ReactJS",
    img: "https://img.icons8.com/color/512/react-native.png",
    rating: 15,
  },
];
</script>

<template>
  <v-container>
    <v-row>
      <v-col v-for="(item, index) of frameList" :key="index">
        <FrameworkPop
          :name="item.name"
          :img="item.img"
          :rating="item.rating"
        ></FrameworkPop>
      </v-col>
    </v-row>
  </v-container>
</template>
