<template>
  <div id="app">
    <!-- testata della pagina -->
    <Header />
    <!-- /testata della pagina -->

    <!-- corpo della pagina -->
    <main>
      <Products />
    </main>
    <!-- /corpo della pagina -->

    <!-- chiusura della pagina -->
    <Footer />
    <!-- /chiusura della pagina -->
  </div>
</template>

<script>
import Header from './components/Header';
import Products from './components/Products';
import Footer from './components/Footer';

export default {
  name: 'App',
  components: {
    Header,
    Products,
    Footer
  }
}
</script>

<style lang="scss">
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>