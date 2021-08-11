<template>
  <h1>Choisissez une salle à réserver</h1>
  <main id="app">
    <section class="products">
      <Product
        v-for="product in products"
        :product="product"
      />
    </section>
  </main>
</template>

<script>
import Product from '../components/Product'

export default {
  name: 'app',
  components: {
    Product
  },
  data () {
    return {
      products: [
        {
          title: 'salle 1',
          color: 'green',
          src: require('../assets/reunion1.jpg')
        },
        {
          title: 'salle 2',
          color: 'red',
          src: require('../assets/reunion2.jpg')
        },
        {
          title: 'salle 3',
          color: 'blue',
          src: require('../assets/reunion3.jpg')
        },
        {
          title: 'salle 4',
          color: 'red',
          src: require('../assets/reunion4.jpg')
        },
        {
          title: 'salle 5',
          color: 'red',
          src: require('../assets/reunion5.jpg')
        }
      ]
    }
  }
}
</script>

<style>

* {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
}

body {
    font-family: 'montseratt', sans-serif;
}

main {
    width: auto;
    min-height: 30vw;
    overflow: hidden;

    display: flex;
    justify-content: center;
    align-items: center;
}

.products {
  display: flex;
  max-width: 2000px;
  padding: 25px;
  margin: auto;
}

h1 {
  padding: 25px;
  text-align: center;
}

</style>