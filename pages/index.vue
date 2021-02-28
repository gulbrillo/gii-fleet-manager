<template>
  <v-container>
    <v-row>
      <v-col>
        <div class="headline pt-4">Funding run: let's make all the money!</div>
        <div class="subtitle-1">August 7, 2021 - 3:00 pm EST</div>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-sheet rounded="lg" style="overflow: hidden" >
          <v-expansion-panels flat >
            <v-expansion-panel >
              <v-expansion-panel-header color="transparent">
                Description
              </v-expansion-panel-header>
              <v-expansion-panel-content color="transparent">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-sheet>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="3">
        <v-sheet rounded="lg">
          <v-list color="transparent" >

            <v-list-item
              color="secondary"
              link
            >
              <v-list-item-avatar>
                <v-icon color="accent">
                  mdi-view-grid-outline
                </v-icon>
              </v-list-item-avatar>
              <v-list-item-content>
                <v-list-item-title>
                  Fleet overview
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-divider class="my-2"></v-divider>

            <v-list-item
              link
              to="/"
              color="secondary"
            >
              <v-list-item-content>
                <v-list-item-title>Mercury Star Runner</v-list-item-title>
                <v-list-item-subtitle>1 spot</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>

            <v-list-item
              link
              color="secondary"
            >
              <v-list-item-content>
                <v-list-item-title>Caterpillar</v-list-item-title>
                <v-list-item-subtitle>fully crewed</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>

            <v-list-item
              link
              color="secondary"
            >
              <v-list-item-content>
                <v-list-item-title>Carrack</v-list-item-title>
                <v-list-item-subtitle>3 spots</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>

            <v-divider class="my-2"></v-divider>

            <v-list-item
              link
              color="secondary"
            >
              <v-list-item-avatar>
                <v-icon color="accent">
                  mdi-view-grid-plus-outline
                </v-icon>
              </v-list-item-avatar>
              <v-list-item-content>
                <v-list-item-title>
                  Add ship
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-sheet>
      </v-col>

      <v-col cols="9">
        <v-sheet
          style="overflow: hidden;"
          min-height="70vh"
          rounded="lg"
        >
          <v-img
            :src="require(`~/assets/msr.png`)"
            gradient="to top, rgba(0,0,0,.3), rgba(0,0,0,.7)"
            height="200"
            class="grey darken-4"
          >
            <v-card color="transparent" flat dark>
              <v-card-title>Mercury Star Runner</v-card-title>
              <v-card-text>
                Cargo capacity: 114 SCU<br>
                Crew: 2 - 3
              </v-card-text>
            </v-card>
          </v-img>

          <v-card flat>
            <v-card-title>
              Crew
            </v-card-title>
            <v-card-text>
              <v-row>
                <v-col cols="6">DasEck (Pilot)</v-col>
                <v-col cols="6">Division Master, Industry</v-col>
              </v-row>
              <v-row>
                <v-col cols="6">Koala (Turret gunner, top)</v-col>
                <v-col cols="6">Ship Master, Security</v-col>
              </v-row>
            </v-card-text>
          </v-card>

          <v-card flat >
            <v-card-title>
              Join the crew
            </v-card-title>
            <v-card-text>
              <v-row>
                <v-col cols="6">
                  <v-select
                    :items="items"
                    label="Position"
                    dense
                    outlined
                ></v-select>
                </v-col>
                <v-col cols="6">
                  <v-btn color="secondary">Enlist</v-btn>
                </v-col>
              </v-row>
            </v-card-text>

          </v-card>

        </v-sheet>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    items: ['Co-pilot', 'Turret gunner, bottom']
  }),
  components: {
  }
}
</script>
