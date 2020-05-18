

<template>
  <v-app>
    <v-app-bar
      app
      color="dark"
      dark
    >
       <v-btn class="mx-2" fab dark color="teal">
      <v-icon dark>mdi-format-list-bulleted-square</v-icon>
    </v-btn>
    </v-app-bar>
    <v-content>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
