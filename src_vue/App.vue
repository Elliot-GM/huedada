<template>
  <div id="nav">
    <header>
      <Navbar />
    </header>
  </div>
  <router-view/>
</template>

<script>
import Navbar from './components/Navbar';

export default {
  name: 'app',
  components: {
    Navbar
  }
}
</script>

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'monsterrat', sans-serif;
  background-color: #EEE;
}

header {
  width: 100vw;
  background-color: Black;
  padding: 20px;
}
</style>
