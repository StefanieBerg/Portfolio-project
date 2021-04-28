<template>
  <v-main>
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
    
  </v-main>
</template>

<script>
  export default {
    name: 'Footer',

    data() {
      return {
        icons: [
            
        ]
      };
    }
  };
</script>

<style lang="scss">
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
  color:aqua;
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
