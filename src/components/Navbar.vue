<template>
<div>
  <b-navbar toggleable="lg" type="dark" variant="dark">
    <b-navbar-brand href="#"><img thumbnail fluid :src="require('../assets/YeiLogo.png')" alt="Image 3" width="25px" height="25px"></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item :to="{name: 'Home'}">Inicio</b-nav-item>
        <b-nav-item>Informacion</b-nav-item>
        <b-nav-item :to="{name: 'About'}">Acerca de</b-nav-item>
        <b-nav-item href="#">Contacto</b-nav-item>
      </b-navbar-nav>
    <b-navbar-nav>
        <b-nav-item-dropdown text="Portafolio" right>
          <b-dropdown-item href="#">Publicidad</b-dropdown-item>
          <b-dropdown-item href="#">Maternidad</b-dropdown-item>
          <b-dropdown-item href="#">Bodas</b-dropdown-item>
          <b-dropdown-item href="#">Familia</b-dropdown-item>
          <b-dropdown-item href="#">Glam</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
.navbar {
    padding: 0;
}
</style>
