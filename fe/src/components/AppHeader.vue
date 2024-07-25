<template>
  <nuxt-ui-container>
    <nuxt-ui-row class="container-header">
      <nuxt-ui-col class="logo-col">
        <img alt="Logo" src="../assets/marketscout-logo.png" class="logo" />
      </nuxt-ui-col>
      <nuxt-ui-col class="nav-col">
        <nav>
          <nuxt-link to="/">Home</nuxt-link>
          <nuxt-link to="/mapping">Mapping and Location Search</nuxt-link>
          <nuxt-link to="/demographics">Consumer Demographics Analysis</nuxt-link>
          <nuxt-link to="/trends">Retail Trend Prediction</nuxt-link>
          <nuxt-link to="/integration">Economic and Social Data Integration</nuxt-link>
          <nuxt-link to="/dashboard">Analytics Dashboard</nuxt-link>
          <nuxt-link to="/monitoring">Real-time Monitoring</nuxt-link>
        </nav>
      </nuxt-ui-col>
      <nuxt-ui-col class="button-col">
        <nuxt-ui-button class="get-started-button" color="lime" outline>
          Get Started
        </nuxt-ui-button>
      </nuxt-ui-col>
    </nuxt-ui-row>
  </nuxt-ui-container>
</template>

<script>
export default {
  name: 'AppHeader'
}
</script>

<style scoped>
.container-header {
  display: flex;
  flex-direction: row;
  align-items: center;
  column-gap: 1rem;
  margin: 0 auto; /* Pusatkan konten secara horizontal */
  width: 100%; /* Mengisi lebar kontainer */
  padding: 10px;
} 

.logo-col {
  width: 10%;

}

.logo {
  height: 80px;
}

.nav-col {
  width: 80%;

}

nav {
  display: flex;
  flex-wrap: wrap; /* Menambahkan flex-wrap */
  gap: 2.5rem; /* Menambahkan jarak antar elemen nav */
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  font-size:larger;
  font-weight: 500;
  color: black;
}
nav nuxt-link {
  text-decoration: none;
  color: inherit;
  transition: color 0.3s; /* Menambahkan transisi untuk efek hover */
}
nav nuxt-link:hover {
  color: lime; /* Menambahkan efek hover warna lime */
}

.button-col {
  width: 10%;
  padding-right: 20px;
}

.get-started-button {
  color: lime; /* Warna teks tombol */
  border: 2px solid lime; /* Warna outline tombol */
  border-radius: 25px; /* Membulatkan sudut tombol */
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Shadow tombol */
  transition: background-color 0.3s, color 0.3s, border-color 0.3s; /* Transisi halus untuk hover */
  padding: 0.5rem 1rem; /* Menambahkan padding pada tombol */
}
.get-started-button:hover {
  background-color: lime; /* Warna latar belakang saat hover */
  color: #fff; /* Warna teks saat hover */
  border-color: lime; /* Warna outline saat hover */
}
</style>
