<template>
  <div>
    <v-app-bar
        app
        elevation="0"
        color="#20232A"
        fixed
    >

      <h1 class="navbar-brand">
        Lunaks
      </h1>


      <v-spacer></v-spacer>
      <v-app-bar-nav-icon class="navigation-icon" @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-menu>
        <template v-slot:activator="{ on, attrs }">
          <v-btn
              rounded
              class="navbar-item d-none d-sm-flex"
              v-bind="attrs"
              v-on="on"
          >Info
          </v-btn>
        </template>
        <v-list>
          <v-list-item
              v-for="(item, index) in items"
              :key="index"
          >
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
      <v-btn rounded class="navbar-item d-none d-sm-flex">Why Lunaks?</v-btn>
      <v-btn rounded class="navbar-item d-none d-sm-flex">Join</v-btn>
    </v-app-bar>

    <v-navigation-drawer
        v-model="drawer"
        fixed
        temporary
        width="200px"
    >
    </v-navigation-drawer>

  </div>
</template>

<script>
export default {
  name: "Navbar",
  data: () => ({
    items: [
      {title: 'info 1'},
      {title: 'info 2'},
      {title: 'info 3'}
    ],
    drawer: null
  })
}
</script>

<style scoped>
li {
  display: inline;
  padding-left: 15px;
  font-size: 1.25em;
}

.navbar-item {
  margin-left: 15px;
}

.navbar-brand {
  color: white;
}

@media screen and (max-width: 500px) {
  .navbar-brand {
    font-size: 20px;
  }
}

@media screen and (min-width: 600px) {
  .navigation-icon {
    display: none;
  }
}
</style>