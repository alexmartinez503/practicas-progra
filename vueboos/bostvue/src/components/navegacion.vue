<template>
   <div>
  <b-navbar toggleable="lg" type="dark" variant="dark">
    <b-navbar-brand href="#">NavBar</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>


      <b-navbar-nav>
        <b-nav-item to="/">home</b-nav-item>
        <b-nav-item to="/about">about</b-nav-item>
        <b-nav-item to="/nuevo">titulo</b-nav-item>

      </b-navbar-nav>

  </b-navbar>
  <router-view/>
</div>


</template>

<script>
export default {
    name: 'navegacion'
}
</script>