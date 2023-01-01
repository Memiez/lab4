<script setup lang="ts">
import MyProfile from "@/components/MyProfile.vue";
</script>

<template>
  <v-container>
    <v-row>
      <v-col>
        <MyProfile></MyProfile>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-table theme="dark">
          <thead>
            <tr>
              <th class="text-left">Name</th>
              <th class="text-left">Calories</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in desserts" :key="item.name">
              <td>{{ item.name }}</td>
              <td>{{ item.calories }}</td>
            </tr>
          </tbody>
        </v-table>
      </v-col>
    </v-row>
  </v-container>
</template>
