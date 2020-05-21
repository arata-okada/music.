<template>
  <v-app>
    <v-app-bar app color="pink" dark>
      <v-toolbar-title class="headline text-uppercase">
        <span @click="$router.push('/')">music .</span>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn to="/" text>
        <span class="mr-2">home</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-content>
      <router-view />
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    //
  })
};
</script>

<style scoped>
.headline span {
  cursor: pointer;
}
</style>