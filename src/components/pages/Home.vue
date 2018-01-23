<template>
  <v-container fluid>
    <v-slide-y-transition mode="out-in">
      <v-layout column align-center>
        <v-card class="card">
          <v-card-media
            class="white--text"
            height="200px"
            src="/static/img/section.jpg"
          >
            <v-container fill-height fluid>
              <v-layout fill-height>
                <v-flex xs12 align-end flexbox>
                  <span class="headline">PWA template</span>
                </v-flex>
              </v-layout>
            </v-container>
          </v-card-media>
          <v-card-title>
            <div>
              <p>This site is a PWA (Progressive Web Application) made in Vue.js</p>
            </div>
          </v-card-title>
          <v-card-actions>
            <v-btn flat color="orange" href="https://github.com/BuissonReda/pwa-template">Check the github of this site</v-btn>
            <v-btn flat color="orange" href="https://vuetifyjs.com/pre-made-themes">Check other templates from vuetify</v-btn>
          </v-card-actions>
        </v-card>
      </v-layout>
    </v-slide-y-transition>
  </v-container>
</template>

<script>
import Api from '../../services/api'
import { EventBus } from '../../event_bus/event_bus'

const api = new Api()

export default {
  name: 'Home'
}
</script>

<style lang="scss" scoped>
.card {
  margin-top: 100px;
}
</style>


