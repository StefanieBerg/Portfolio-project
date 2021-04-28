
<template>
  <v-content>
    
  <div class="projects">
    <h2>My projects</h2>
  </div>

  <div class="startText">
    <p>Here I have selected some of my previous projects to show you. 
       Most of these projects have been made in connection with my education at EASV.</p> 
    </div>

    <v-container>
    <div class="galleryBlock">
      <h2 class="text-center">Photography</h2>
      <div class="startText">
        <p><span class="phat-text">Photography</span> is definitely one of the things I spend part of my free time on and I always try to <span class="phat-text">get better</span> at it.
          I really like taking pictures. Especially of <span class="phat-text">animals</span>, which I definitely take the most pictures of. But I am always <span class="phat-text">open to new challenges</span> and <span class="phat-text">learning something new</span>.
          Here you can see a small selection of the pictures I have taken:</p> 
      </div>
        <v-row>
          <v-col
            v-for="item in items"
            :key="item.id"
            class="d-flex child-flex"
            cols="6" md="4">

            <v-img
              :src="item.src"
              aspect-ratio="1"
              class="grey lighten-2">

            <template v-slot:placeholder>
              <v-row
                class="fill-height ma-0"
                align="center"
                justify="center">

            <v-progress-circular
              indeterminate
              color="grey lighten-5">
            </v-progress-circular>
          </v-row>
        </template>
      </v-img>
    </v-col>
  </v-row>
  </div>
  </v-container>

  <div class="brochureBlock"> 
    <h3>Brochure about esbjerg</h3>

    <div class="startText">
    <p>In our first semester, we had to make an <span class="phat-text">info-folder</span> about a district in Esbjerg.
      The group I was in chose the districts <span class="phat-text">Sædding</span> and <span class="phat-text">Hjerting</span>, which lay right next
      to the North Sea. For this project we did <span class="phat-text">research</span> on the two districts and 
      were out <span class="phat-text">taking pictures</span> of the attractions. We chose that our design for the folder should be <span class="phat-text">minimalistic</span>.</p> 
    </div>

    <div class="strandvejenBrochure">
    <div class="column">
      <img src="../assets/images/strandvejen1.jpg">
    </div>
    <div class="column">
      <img src="../assets/images/strandvejen2.jpg">
    </div>
    </div>

    <h3>Poster about Esbjerg</h3>
    <div class="startText">
    <p>In addition to our info-folder we also had to make a <span class="phat-text">poster</span>.
       Our poster is inspired by the posters with Danish cities, and shows 
       the <span class="phat-text">sculpture "Men at Sea"</span> and the <span class="phat-text">beach</span>.</p> 
    </div>
    <div  class="poster">
      <div class="column">
      <img src="../assets/images/poster.jpg">
      </div>
    </div>
  </div>

  <div class="examProject">
   <h3>Exam project</h3>
    <div class="startText">
    <p>For our first semesters exam project we had to make an <span class="phat-text">interactive teaching/science 
      application</span> about the sea. The group I was in made a <span class="phat-text">website</span> where you could learn
      about corals and adopt one. By adopting a coral you would help <span class="phat-text">protect the coral reefs</span>.</p> 
    </div>
    <div  class="website">
      <div class="columnWebsite">
      <img src="../assets/images/Eksamensprojekt1.jpg">
      </div>
    </div>
     <div  class="website">
      <div class="columnWebsite">
      <img src="../assets/images/Eksamensprojekt3.jpg">
      </div>
    </div>
    </div>

    <div class="posterBlock"> 
    <h3>Brochure about esbjerg</h3>
    <div class="startText">
    <p>In the first semester we had to make a <span class="phat-text">poster</span>. I made a poster with lyrics 
      from <span class="phat-text">Spring Day by BTS</span>. The lyrics are both the original in Korean and 
      translated into English.</p> 
    </div>
     <div  class="poster">
      <div class="column">
      <img src="../assets/images/BTSposter.jpg">
      </div>
      </div>
    </div>

   <footer>
      <div class="footer-content">
        <ul class="socials">
          <li><a href="https://www.facebook.com/stefanieberg.breintoft"><i class="fab fa-facebook"></i></a></li>
          <li><a href="https://twitter.com/stefberg_"><i class="fab fa-twitter"></i></a></li>
          <li><a href="https://www.linkedin.com/in/stefaniebergbreintoft/"><i class="fab fa-linkedin"></i></a></li>
          <li><a href="https://www.instagram.com/bstefanieb/"><i class="fab fa-instagram"></i></a></li>
        </ul>
      </div>
      <div class="footer-bottom">
        <p>copyright &copy;2021 Stefanie Berg Breintoft</p>
      </div>
    </footer>

  </v-content>
</template>

<script>
export default {
  name: "My projects",

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
         {
          id: 7,
          src: require("../assets/images/img7.jpg")
        },
         {
          id: 6,
          src: require("../assets/images/img9.jpg")
        },
         {
          id: 6,
          src: require("../assets/images/img10.jpg")
        },
      ]
    };
  }
};
</script>

<style lang="scss">
.projects {
  margin-left: 30px;
  margin-top: 20px;
  margin-bottom: 20px;
}

.galleryBlock {
  margin-bottom: 30px;
  margin-left: 10px;
  margin-right: 10px;
}

.brochureBlock {
  background-color: #403F3F;
}
.brochureBlock h3 {
  color: #f5f5f5;
  display: flex;
  justify-content: center;
  padding-top: 20px;
  font-size: 25px;
}
.brochureBlock p {
  color: #f5f5f5;
}

.strandvejenBrochure {
  display: flex;
  justify-content: center;
}
.column img {
  height: 270px;
  width: 210px;
  margin-left: 50px;
  margin-bottom: 30px;
}

.poster {
  display: flex;
  justify-content: center;
}

.examProject h3 {
  display: flex;
  justify-content: center;
  padding-top: 20px;
  font-size: 25px;
}
.website {
  display: flex;
  justify-content: center;
}
.columnWebsite img {
  height: 270px;
  width: 450px;
  margin-left: 50px;
  margin-bottom: 30px;
}

.posterBlock {
  background-color: #403F3F;
}
.posterBlock h3 {
  color: #f5f5f5;
  display: flex;
  justify-content: center;
  padding-top: 20px;
  font-size: 25px;
}
.posterBlock p {
  color: #f5f5f5;
}
</style>
