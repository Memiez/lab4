<script setup lang="ts">
import {
  mdiFaceWomanShimmerOutline,
  mdiAccountDetailsOutline,
  mdiDuck,
  mdiAccountSchoolOutline,
  mdiMusicNotePlus,
} from "@mdi/js";
</script>

<template>
  <v-container>
    <v-row>
      <v-col>
        <v-card class="mx-auto" max-width="350" variant="outlined">
          <v-img
            class="align-end text-white"
            height="400"
            src="https://i.chzbgr.com/full/9442674176/h7E3950EA/one-bossy-mama"
            cover
          >
            <v-card-title>Hello, I'm Meow Meow</v-card-title>
          </v-img>
        </v-card>

        <v-row justify="center">
          <v-col cols="6">
            <v-table>
              <thead>
                <tr>
                  <th>Ms. Meow Meow</th>
                  <th>Contact</th>
                </tr>
                <tr>
                  <td>Position</td>
                  <td>Address:</td>
                </tr>
                <tr>
                  <td>ใส่ๆ เข้าไป</td>
                  <td>Phone :</td>
                </tr>
                <tr>
                  <td>ใส่อีก</td>
                  <td>Email :</td>
                </tr>
              </thead>
            </v-table>
          </v-col>
        </v-row>

        <v-timeline>
          <v-timeline-item dot-color="purple-lighten-2" fill-dot>
            <v-card>
              <v-card-title class="bg-purple-lighten-2">
                <v-icon
                  size="large"
                  class="mr-4"
                  :icon="mdiFaceWomanShimmerOutline"
                ></v-icon>
                <h2 class="font-weight-light">About Me</h2>
              </v-card-title>
              <v-card-text>
                Lorem ipsum dolor sit amet, no nam oblique veritus. Commune
                scaevola imperdiet nec ut, sed euismod convenire principes at.
                Est et nobis iisque percipit.
              </v-card-text>
            </v-card>
          </v-timeline-item>

          <v-timeline-item dot-color="amber-lighten-1" fill-dot size="x-small">
            <v-card>
              <v-card-title class="bg-amber-lighten-1 justify-end">
                <h2 class="mr-4 font-weight-light">Experience</h2>
                <v-icon size="large" :icon="mdiAccountDetailsOutline"></v-icon>
              </v-card-title>
              <v-card-text>
                Lorem ipsum dolor sit amet, no nam oblique veritus. Commune
                scaevola imperdiet nec ut, sed euismod convenire principes at.
                Est et nobis iisque percipit.
              </v-card-text>
            </v-card>
          </v-timeline-item>

          <v-timeline-item dot-color="cyan-lighten-1" fill-dot>
            <v-card>
              <v-card-title class="bg-cyan-lighten-1">
                <v-icon class="mr-4" size="large" :icon="mdiDuck"></v-icon>
                <h2 class="font-weight-light">Skills</h2>
              </v-card-title>
              <v-card-text>
                Lorem ipsum dolor sit amet, no nam oblique veritus. Commune
                scaevola imperdiet nec ut, sed euismod convenire principes at.
                Est et nobis iisque percipit.
              </v-card-text>
            </v-card>
          </v-timeline-item>

          <v-timeline-item dot-color="red-lighten-1" fill-dot size="x-small">
            <v-card>
              <v-card-title class="bg-red-lighten-1 justify-end">
                <h2 class="mr-4 font-weight-light">Education</h2>
                <v-icon size="large" :icon="mdiAccountSchoolOutline"></v-icon>
              </v-card-title>
              <v-card-text>
                Lorem ipsum dolor sit amet, no nam oblique veritus. Commune
                scaevola imperdiet nec ut, sed euismod convenire principes at.
                Est et nobis iisque percipit.
              </v-card-text>
            </v-card>
          </v-timeline-item>

          <v-timeline-item dot-color="green-lighten-1" fill-dot>
            <v-card>
              <v-card-title class="bg-green-lighten-1">
                <v-icon
                  class="mr-4"
                  size="large"
                  :icon="mdiMusicNotePlus"
                ></v-icon>
                <h2 class="font-weight-light">Hobby</h2>
              </v-card-title>
              <v-card-text>
                Lorem ipsum dolor sit amet, no nam oblique veritus. Commune
                scaevola imperdiet nec ut, sed euismod convenire principes at.
                Est et nobis iisque percipit.
              </v-card-text>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </v-col>
    </v-row>
  </v-container>
</template>
