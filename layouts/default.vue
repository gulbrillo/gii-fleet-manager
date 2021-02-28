<template>
  <v-app id="inspire">
    <v-app-bar
      app
      color="white"
    >
      <v-container class="py-0 fill-height">
        <v-avatar
          class="mr-10"
          color="grey darken-1"
          size="32"
        >
          <img :src="require(`~/assets/garden.png`)" alt="logo">
        </v-avatar>

        <v-responsive max-width="260">
          <v-text-field
            dense
            flat
            hide-details
            rounded
            solo-inverted
            label="search"
          ></v-text-field>
        </v-responsive>

        <v-spacer></v-spacer>

        <v-btn
          link
          text
          color="primary"
        >
          Members
        </v-btn>

        <v-btn
          to="/"
          text
          color="primary"
        >
          Events
        </v-btn>

        <v-btn
          link
          text
          color="primary"
        >
          Profile
        </v-btn>

      </v-container>
    </v-app-bar>

    <v-main class="grey lighten-3">
      <nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      title: 'Vuetify.js'
    }
  }
}
</script>
