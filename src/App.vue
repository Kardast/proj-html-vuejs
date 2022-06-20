<template>
  <div id="app">

    <!-- Header -->
    <header>

      <MyHeader 
      :headerSocial="mySocials"
      :headerLinks="myLinks"
      />
    </header>

    <!-- Jumbrotron -->
    <section>

      <MyJumbo/>
    </section>

    <!-- Main -->
    <main>

      <!-- Main will be divided in 5 similar sections -->
      <!-- Section 1 Award-->
      <section>

        <MyAwardSection/>
      </section>

      <!-- Section 2 Full-Service -->
      <section>

        <MyServiceSolution/>
      </section>

      <!-- Section 3 Move -->
      <section>

        <MyMoveEase/>
      </section>

      <!-- Section 4 Testimonials -->
      <section>

        <MyTestimonials/>
      </section>

      <!-- Section 5 Request quote -->
      <section>

        <MyRequestQuote/>
      </section>
    </main>

    <!-- Footer -->
    <footer>

    </footer>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbo from './components/MyJumbo.vue'
import MyAwardSection from './components/MyAwardSection.vue'
import MyServiceSolution from './components/MyServiceSolution.vue'
import MyMoveEase from './components/MyMoveEase.vue'
import MyTestimonials from './components/MyTestimonials.vue'
import MyRequestQuote from './components/MyRequestQuote.vue'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbo,
    MyAwardSection,
    MyServiceSolution,
    MyMoveEase,
    MyTestimonials,
    MyRequestQuote
  },

  data(){
    return{
      mySocials: [
        {
          social: "fa-brands fa-facebook-f"
        },
        {
          social: "fa-brands fa-twitter"
        },
        {
          social: "fa-brands fa-instagram"
        },
        {
          social: "fa-brands fa-youtube"
        }
      ],

      myLinks: [
        {
          link: "Home",
        },
        {
          link: "Rates",
        },
        {
          link: "Testimonials",
        },
        {
          link: "FAQ",
        },
        {
          link: "Blog",
        },
        {
          link: "Contact",
        },
      ]
    }
  }
}
</script>

<style lang="scss">
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

}
</style>
