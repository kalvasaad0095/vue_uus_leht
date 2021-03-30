<template>
      <div class="heroBlock">
 <v-carousel hide-delimiters cycle >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    >
     <v-row class="title fill-height hidden-xs-only" align="center" justify="center">{{ item.title }}</v-row>
        </v-carousel-item>
  </v-carousel>
      </div>
  
</template>

<script>
  export default {
    name: 'Hero',

    data: () => {
      return {
        items: [
          {
            src: "https://www.wallpaperup.com/uploads/wallpapers/2019/08/16/1335206/d973ae84195430a6e9845827d3918725.jpg",
            title: "The science of today is the technology of tomorrow",
          },
          {
            src: 'https://images.squarespace-cdn.com/content/v1/597886853a04111fe3d04c1f/1502298125342-6X0JKOSHCMU4DH104SUC/ke17ZwdGBToddI8pDm48kO5yXVzgNH97Y0stbOL7oGV7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z5QPOohDIaIeljMHgDF5CVlOqpeNLcJ80NK65_fV7S1UaLvKKTEpoHa_vHy8M3FKbzHg68KZsWZks1yKvfKtyhIq48P6Er5hTXB8mTK70lUqQ/design-header.jpg?format=2500w',
              title: "Design is intelligence made visible",
          },
          {
            src: 'https://wallpaper.dog/large/10724660.jpg',
              title: "Technology is best when it brings people together",
          },
          {
            src: 'https://i.redd.it/2r8wyj33q5g31.png',
              title: "We must act out passion before we can feel it",
          },
        ],
      }
    },
  }
</script>