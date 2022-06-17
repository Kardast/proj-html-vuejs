<template>
  <div id="app">

    <!-- Header -->
    <header>

      <MyHeader />
    </header>

    <!-- Jumbrotron -->
    <section>

    </section>

    <!-- Main -->
    <main>

      <!-- Main will be divided in 5 similar sections -->
      <!-- Section 1 Award-->
      <section>

      </section>

      <!-- Section 2 Full-Service -->
      <section>

      </section>

      <!-- Section 3 Move -->
      <section>

      </section>

      <!-- Section 4 Testimonials -->
      <section>

      </section>

      <!-- Section 5 Request quote -->
      <section>

      </section>
    </main>

    <!-- Footer -->
    <footer>
      
    </footer>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'

export default {
  name: 'App',
  components: {
    MyHeader
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
