<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div>
  <nav class="navbar navbar-expand-lg navbar-light">
    <a class="navbar-brand yuji" href="#">Jeffrey Sanchez</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarText" aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse justify-content-end questrial" id="navbarText">
      <ul class="navbar-nav">
        <li class="nav-item active">
          <RouterLink class="nav-link" to="/">Home</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/about">About</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/service">Service</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/contact">Contact</RouterLink>
        </li>
      </ul>
    </div>
  </nav>

  <RouterView class="contentArea" />
  </div>
</template>

<style scoped>
nav {
  padding-left: 100px;
  padding-right: 100px;
  font-size: 13pt;
  background-color: white;
}
.navbar-brand {
  font-size: 25pt;
}
.contentArea {
  padding: 0px 250px 100px 250px;
  display: flex;
  justify-content: center;
  flex-direction: column;
}
nav a {
  text-decoration: none;
}
</style>
