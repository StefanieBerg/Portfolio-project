<template>
  <v-container>
    <div class="block galleryBlock">
      <h2 class="text-center">Mine billeder</h2>
      <v-row>
    <v-col
      v-for="item in items"
      :key="item.id"
      class="d-flex child-flex"
      cols="4"
    >
      <v-img
        :src="item.src"
        aspect-ratio="1"
        class="grey lighten-2"
      >
        <template v-slot:placeholder>
          <v-row
            class="fill-height ma-0"
            align="center"
            justify="center"
          >
            <v-progress-circular
              indeterminate
              color="grey lighten-5"
            ></v-progress-circular>
          </v-row>
        </template>
      </v-img>
    </v-col>
  </v-row>
    </div>
  </v-container>
</template>

<script>
  export default {
    name: 'Gallery',

    data() {
      return {
        items: [
        {
          id: 1,
          src: require("../assets/images/img1.jpg")
        },
        {
          id: 2,
          src: require("../assets/images/img2.jpg")
        },
        {
          id: 3,
          src: require("../assets/images/img3.jpg")
        },
        {
          id: 4,
          src: require("../assets/images/img4.jpg")
        },
        {
          id: 5,
          src: require("../assets/images/img5.jpg")
        },
        {
          id: 6,
          src: require("../assets/images/img6.jpg")
        },
        ]
      };
    }
  };
</script>
