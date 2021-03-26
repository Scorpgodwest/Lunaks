<template>
    <div class="header">
      <v-card width="90%" color="#040D21" class="rounded-lg header-card">
        <v-container>
          <v-row no-gutters>
            <v-col>
              <h1 class="description">The place for your project development</h1>
              <p class="description">блаблаблабла, тут типо описание окда</p>
            </v-col>
            <v-col>
              <div style="display: flex; justify-content: center">
                <img src="../../public/logo.png" class="header-image">
              </div>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </div>
</template>

<script>
export default {
  name: "Header",
  data: () => {
    color: "#040D21"
  }
}
</script>

<style scoped>
.header {
  display: flex;
  justify-content: center;
  margin-top: 15px;
}
.description {
  text-align: center;
  color: white;
}
.header-image {
  width: 300px;
  height: 300px;
}
.header-card {
  background: linear-gradient(to top right, #5693AF, #040D21);
}
@media  screen and (max-width: 500px) {
  .header-image {
    width: 150px;
    height: 150px;
  }
}
</style>