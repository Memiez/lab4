<template>
  <v-app :theme="theme">
    <v-app-bar>
      <v-spacer></v-spacer>

      <v-btn
        :prepend-icon="theme === 'light' ? mdiWeatherSunny : mdiWeatherNight"
        @click="onClick"
      >
        Toggle Theme</v-btn
      >
    </v-app-bar>

    <v-navigation-drawer expand-on-hover rail permanent>
      <v-list>
        <v-list-item
          prepend-avatar="https://i.pinimg.com/originals/b2/e7/56/b2e756d9e02a17daf195ea4927494ecd.gif"
          title="Gudetama"
          subtitle="sandra_a88@gmailcom"
        ></v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item
          :prepend-icon="mdiFolder"
          title="My Files"
          value="myfiles"
          to="/my-files-view"
        ></v-list-item>
        <v-list-item
          :prepend-icon="mdiAccountMultiple"
          title="Profile Page"
          value="profile"
          to="/profile-page"
        ></v-list-item>
        <v-list-item
          :prepend-icon="mdiStar"
          title="Starred"
          value="starred"
          to="starred"
        ></v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
import { ref } from "vue";
import {
  mdiFolder,
  mdiAccountMultiple,
  mdiStar,
  mdiWeatherSunny,
  mdiWeatherNight,
  mdiEmoticonKissOutline,
  mdiVuetify,
} from "@mdi/js";

const theme = ref("light");

function onClick() {
  theme.value = theme.value === "light" ? "dark" : "light";
}
</script>
