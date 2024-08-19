<script setup>
import { RouterLink } from 'vue-router';
</script>

<template>
    <header>
        <nav2 class="container">
        </nav2>
        <nav class="container">
            <div class="branding">
                <ul class="nav-routes">
                    <RouterLink to="/">Inicio</RouterLink>
                    <RouterLink to="/donations">Donaciones</RouterLink>
                    <RouterLink to="/services">Servicios</RouterLink>
                    <RouterLink to="/resources">Recursos</RouterLink>
                    <RouterLink to="/blog">Blog</RouterLink>
                    <RouterLink to="/merch">Mercancia</RouterLink>
                    <RouterLink to="/collaborators">Colaboradores</RouterLink>
                </ul>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header {
  background-color: #272b00;
  nav {
    display: flex;
    align-items: center;
    padding: 20px 50px;

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 50px;
      list-style: none;

      a {
        text-decoration: none;
        color: #f9fbca;
      }
    }
  }
  nav2 {
    display: flex;
    align-items: center;
    padding: 100px;
    background-color: #bec092;
    min-width: 100%;
    width: auto;
  }
}
</style>