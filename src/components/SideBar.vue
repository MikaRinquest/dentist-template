<template>
  <nav>
    <v-navigation-drawer
      v-model="drawer"
      dark
      app
      mini-variant
      mini-variant-width="100"
      class="teal"
    >
      <v-list>
        <v-list-item>
          <v-list-item-content>
            <v-icon class="mb-2" large>fas fa-hand-holding-medical</v-icon>
            <v-list-item-subtitle align="center">Medi</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list flat>
        <v-list-item router to="/"></v-list-item>
        <v-list-item-content>
          <v-icon class mb-2> fas fa-home</v-icon>
        </v-list-item-content>
        <v-list-item router to="/">
          <v-badge color="pink" dot overlap>
            <v-list-item-content>
              <v-icon class="mb-2"> fas fa-user</v-icon>
            </v-list-item-content>
          </v-badge>
        </v-list-item>
        <v-list-item router to="/">
          <v-list-item-content>
            <v-icon class="mb-2">fas fa-envelope</v-icon>
          </v-list-item-content>
        </v-list-item>
        <v-list-item router to="/">
          <v-list-item-content>
            <v-icon class="mb-2">fas fa-cog</v-icon>
          </v-list-item-content>
        </v-list-item>
        <v-list-item router to="/">
          <v-list-item-content>
            <v-icon class="mb-2">fas fa-question-circle</v-icon>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>
<script>
export default {
  data: () => ({
    drawer: true,
  }),
};
</script>
