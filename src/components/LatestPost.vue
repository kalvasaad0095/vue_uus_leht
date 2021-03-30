<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">Some of my works</h2>
      <v-row>
        <v-col v-for="item in items" :key="item.id" cols="12" md="4">
          <v-card outlined class="mx-auto">
            <v-img
              class="white--text align-end"
              height="200px"
              :src="item.src"
            >
              <v-card-title>{{ item.title }}</v-card-title>
            </v-img>
            <v-card-subtitle class="pb-0">{{ item.subtitle }}</v-card-subtitle>
            <v-card-text class="text--primary">
              <div>{{ item.description }}</div>
            </v-card-text>
            <v-card-actions>
              <v-btn color="primary" text> <router-link to='/portfolio'>Click to see</router-link></v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <div class="text-center">
    <v-btn
      rounded
      color="grey"
      dark
     
    >
      <router-link to='/portfolio'>Click for more...</router-link>
    </v-btn>
  </div>
  </div>
  
</template>

<script>
export default {
  name: "LatestPost",
  data: () => ({
    show: false,
    items: [
      {
        id: 1,
        title: "Kiviaiameister",
        subtitle: "www.kiviaiameister.ee",
        description: "",
        src: require("../assets/images/kiviaed.jpg")
      },
      {
        id: 2,
        title: "Kristaphoto",
        subtitle: "www.kristaphoto.se",
        description: "",
        src: require("../assets/images/virmalised.jpeg")
      },
      {
        id: 3,
        title: "Estonia Truth",
        subtitle: "www.estoniatruth.ee",
        description: "",
        src: require("../assets/images/estonia.jpg")
      },
    
    ]
  })
};
</script>