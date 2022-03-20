<template>
  <v-app>
    <v-navigation-drawer app>
    <!-- -->
    </v-navigation-drawer>

    <v-app-bar app>
    <!-- -->
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view />
        <v-btn @click="counter++">
          Click me {{ counter }}
        </v-btn>
      </v-container>
    </v-main>

    <v-footer app>
    <!-- -->
    </v-footer>
  </v-app>
</template>

<script>
import { defineComponent, ref } from '@vue/composition-api'

export default defineComponent({
  setup () {
    const counter = ref(0)
    return { counter }
  }
})
</script>
