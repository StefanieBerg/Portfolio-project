<template>
  <v-main>
    <Hero/>

    <div class="imageMe">
      <img src="../assets/images/Me.jpg">
    </div>

    <div class="startText">
    <p>My name is <span class="phat-text">Stefanie Berg Breintoft</span> and I’m 22 years old. I’m born and raised near a danish city 
        called Esbjerg. I’m currently a <span class="phat-text">multimediadesign student</span> at Business Academy Southwest in 
        Esbjerg and I will finish that in the summer of 2022.</p> 
    </div>

    <div class="startText">
        <p>I’m a <span class="phat-text">passionated</span> and <span class="phat-text">motivated</span> multimediadesign student who has experience with freelance 
        graphic design and amateur photography. I like working <span class="phat-text">targeted</span> and <span class="phat-text">structured</span> with all of my 
        projects, but I can keep calm under stressfull situations with <span class="phat-text">logical thinking</span>.</p>  
    </div>

    <div class="startText">
        <p>Most of the time I enjoy working alone, but I can function well in a group too.
        I have been told before that I contributes to the good mood of the group and is good at <span class="phat-text">getting
        things done</span>.</p> 
    </div>

    <div class="startText">
        <p>Here is my video cv (danish) where I tell you about me and how I like to work:</p>
    </div>

    <div class="videoCV">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Wg1RRIkGPFg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
    </iframe>
  </div>

    <div class="experienceBlock">
      <div>
        <h1>EXPERIENCE</h1>

        <p id="headline">EDUCATION</p>
        <p id="headline">Primary school</p>

        <p>Egekratskolen 2005 - 2012</p>
        <p>Nordre skole 2012 - 2015</p>

        <p id="headline">High school</p>

        <p>Rybners Tekniske Gymnasium 2015 - 2018 </p>
        <p>Chemistry A / Math A </p>

        <p id="headline">UNIVERSITY</p>

        <p>Nursing school 2018 - 2019</p>
        <p>Multimediadesign 2020 - 2022</p>

        <div class="lastSection">
          <p>WANT TO KNOW MORE</p>
          <p>Download my CV</p>
        </div>
      </div>

      <v-btn
        id="button"
        elevation="2"
        color="green">
        <a href="https://www.dropbox.com/s/5onme88tsfxzssb/CV%20Stefanie.pdf?dl=0" target="_blank">
          Download
        </a>
      </v-btn>
    </div>

    <footer>
      <div class="footer-content">
        <ul class="socials">
          <li><a href="https://www.facebook.com/stefanieberg.breintoft" target="_blank"><i class="fab fa-facebook"></i></a></li>
          <li><a href="https://twitter.com/stefberg_" target="_blank"><i class="fab fa-twitter"></i></a></li>
          <li><a href="https://www.linkedin.com/in/stefaniebergbreintoft/" target="_blank"><i class="fab fa-linkedin"></i></a></li>
          <li><a href="https://www.instagram.com/bstefanieb/" target="_blank"><i class="fab fa-instagram"></i></a></li>
        </ul>
      </div>
      <div class="footer-bottom">
        <p>copyright &copy;2021 Stefanie Berg Breintoft</p>
      </div>
    </footer>
  </v-main>
</template>

<script>

import Hero from '../components/Hero';

export default {
  name: "Home",

  components: {
    Hero,
  },

  data() {
    return {
      items: [

      ]
    };
  }
};
</script>

<style lang="scss">

.phat-text {
  font-weight:600;
}

.imageMe {
  clip-path: polygon(20% 0%, 80% 0%, 100% 20%, 100% 80%, 80% 100%, 20% 100%, 0% 80%, 0% 20%);
  height: 250px;
  width: 200px;
  display: block;
  margin: 20px auto;
  background-size: 40%;
}

.imageMe img{
max-width:100%;
max-height:100%;
}

.startText p {
  padding-left: 30px;
  padding-right: 25px;
}

.videoCV {
  display: flex;
  justify-content: center;
  padding-bottom: 20px;
}

.experienceBlock {
  background-color:#403F3F;
  block-size: 700px;

  h1{
  padding: 15px;

  display: flex;
  justify-content: center;
  color: white;
  }

  p{
  display: flex;
  justify-content: center;
  color: white;
  margin: 0%;
  }

  #headline {
    font-size: 25px;
    font-weight: bold;
    margin: 10px;
  }

  .lastSection {
    margin-top: 50px;
    margin-bottom: 10px;
  }

  #button {
  display: block;
  margin-left: auto;
  margin-right: auto;
  }
  #button a {
    text-decoration: none;
    color: white;
  }
}

footer {
  background: #222;
  height: auto;
  width: 100vw;
  padding-top: 20px;
  color: #fff;
}
.footer-content {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  text-align: center;
}
.footer-content h3 {
  font-size: 1.8rem;
  font-weight: 400;
  text-transform: capitalize;
  line-height: 3rem;
}
.footer-content p {
  max-width: 500px;
  margin: 10px auto;
  line-height: 28px;
  font-size: 14px;
}
.socials {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 1rem 0 0 0;
}
.socials li {
  margin: 0 15px;
}
.socials a i {
  font-size: 1.5rem;
  transition: color .4s ease;
  color: white;
  text-decoration: none;
}
.socials a:hover i {
  color:#a2bce6;
}

.footer-bottom {
  background: #222;
  width: 100vw;
  padding: 20px 0;
  text-align: center;
}
.footer-bottom p {
  height: 10px;
  font-size: 14px;
  word-spacing: 2px;
  text-transform: capitalize;
}
</style>
