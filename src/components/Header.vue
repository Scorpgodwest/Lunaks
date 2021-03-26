<template>
    <div class="header">
      <v-card width="90%" color="#040D21" class="rounded-lg">
        <v-container>
          <v-row no-gutters>
            <v-col>
              <h1 class="description">The place for your project development</h1>
              <p class="description">блаблаблабла, тут типо описание окда</p>
            </v-col>
            <v-col>
              <div style="display: flex; justify-content: center">
                <img src="../../public/logo.png" width="300px" height="300px">
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
</style>