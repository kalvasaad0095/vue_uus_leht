<template>
  <v-container>
    <v-footer padless>
      <v-card flat class="text-center">
        <v-card-text>
          <v-btn v-for="icon in icons" :key="icon" class="mx-4" icon>
            <v-icon size="24px">{{ icon }}</v-icon>
          </v-btn>
        </v-card-text>
        <v-card-text
          class="pt-0"
        >Every website needs a Terms and Conditions. Even if your website is not for your business or any commercial structure, you will be better off with a Terms and Conditions agreemnent. All websites are advised to have their own agreements for their own protection.</v-card-text>
        <v-divider></v-divider>
        <v-card-text>
          {{ new Date().getFullYear() }} —
          <strong>KalvarWeb</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-container>
</template>

<script>
export default {
  name: "Footer",
  data: () => ({
    icons: [
      "fab fa-facebook", 
      "fab fa-codepen",
      "fab fa-github",
    ]
  })
};
</script>