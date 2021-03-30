<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/portfolio.png">
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
          <v-col>
            <v-container>
              <div class="headline">Portfolio</div>
            </v-container>
          </v-col>
        </v-row>
      </v-img>
    </div>
    <div class="block">
      <v-container>
        <p>Ea pri vitae antiopam theophrastus, ut sit erat putent eruditi. Qui at mutat adversarium. Postulant delicatissimi ei qui, an nonumy dolorem nam. Cu philosophia instructior pri, nec cu mutat homero saperet, cu paulo ridens legendos has. Cu veri oportere pri, ad integre numquam iudicabit mel. </p>
      </v-container>
    </div>
    <div class="block">
      <v-container>
        <h2 class="text-center">My work</h2>
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
              <v-btn color="primary" text> <router-link to= {item.path}>Visit page</router-link></v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
      </v-container>
    </div>
  </v-content>
</template>

<script>
export default {
  name: "Portfolio",
  data() {
    return {
      items: [
        {
           id: 1,
          src: require("../assets/images/kiviaed.jpg"),
          name: 'Kiviaiameister',
          title: '',
          path: 'www.kiviaiameister.ee',
        },
        {
          id: 2,
          src: require("../assets/images/virmalised.jpeg"),
          name: '',
          title: ''
        },
        {
          id: 3,
          src: require("../assets/images/estonia.jpg"),
          name: '',
          title: ''
        },
          {
          id: 4,
          src: require("../assets/images/matrix.jpg"),
          name: '',
          title: ''
        },

          {
          id: 5,
          src: require("../assets/images/weather.png"),
          name: '',
          title: ''
        }
      ]
    };
  }
};
</script>