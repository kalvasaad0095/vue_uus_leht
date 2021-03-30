<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">About</h2>
      <v-parallax
    dark
   
    src="https://www.theagilityeffect.com/app/uploads/2019/09/00_VINCI-ICONOGRAPHIE_GettyImages-1065377816-1280x680.jpg"
  >
    <v-row
      align="center"
      justify="center"
    >
      <v-col
        class="text-center"
        cols="12"
      >
        <h1 class="display-1 font-weight-thin mb-4">
        KalvarWeb Design
        </h1>
        <h4 class="subheading">
          The place where science, design, technology and passion meet
        </h4>
      </v-col>
    </v-row>
  </v-parallax>
    </v-container>
  </div>
</template>


<script>
  export default {
    name: 'Gallery',

   data: () => ({
      showMenu: false,
      items: [
       
      ],
    }),
  }
</script>
