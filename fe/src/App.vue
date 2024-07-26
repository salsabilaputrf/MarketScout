<template>
  <AppHeader/>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'App',
  components: {
    AppHeader
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex; /* Menambahkan Flexbox */
  flex-direction: column; /* Mengatur arah kolom */
  align-items: center; /* Mengatur elemen agar sejajar di tengah secara horizontal */
  justify-content: flex-start; /* Mengatur elemen agar sejajar di tengah secara vertikal */
  width: 100%;
  max-width: 1900px;
  min-width: 1200px;
  margin: 0 auto; /* Memusatkan elemen secara horizontal */
  height: 100vh; /* Memastikan elemen mengambil tinggi penuh dari viewport */
}


</style>
