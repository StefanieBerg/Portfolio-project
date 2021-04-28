<template>
  <v-content>
     <div class="textContact">
        <p>If you are interested in hearing more about me, 
            then you can contact me by <span class="phat-text">email</span> or <span class="phat-text">phone</span>.
            you can also contact me on my <span class="phat-text">social media</span>.</p>
    </div>

    <div class="boxInfo">
      <div class="contactInfo">
        <p><span class="phat-text">Mail</span>: stefanieb@hotmail.dk</p>
      </div>
      <div class="contactInfo">
        <p><span class="phat-text">Telefonnummer</span>: 31651484</p>
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
  name: "Contact",

  data: () => ({
      valid: true,
      name: '',
      nameRules: [
        v => !!v || 'Name is required',
        v => (v && v.length <= 10) || 'Name must be less than 10 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail is required',
        v => /.+@.+\..+/.test(v) || 'E-mail must be valid',
      ],
      message: '',
      messageRules: [
        v => !!v || 'Message is required',
        v => (v && v.length >= 10) || 'Message must be more than 10 characters',
      ],
    }),

    methods: {
      validate () {
        this.$refs.form.validate()
      },
      reset () {
        this.$refs.form.reset()
      },
    },
};
</script>

<style lang="scss">

  .boxInfo {
    padding-top: 20px;
  }

  .contactInfo {
    display: flex;
    justify-content: center;
  }

  .textContact {
    padding-top: 30px;
    padding-left: 30px;
    padding-right: 25px;
  }

</style>