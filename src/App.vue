<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div alt="Cymbal logo" class="logo" width="125" height="125">Cymbal10</div>

    <div class="wrapper"> 
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/origin">Origin</RouterLink>
        <RouterLink to="/shartinga">shartinga</RouterLink>
        <RouterLink to="/partners">Partners</RouterLink>
      </nav>
    </div> 
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  font-size: 30px;
  font-weight: 600;
  color: var(--color-heading);
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    padding-right: calc(var(--section-gap) / 2); 
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    flex-wrap: wrap;
  }

  nav {
    display: flex;
    text-align: left;
    margin-left: 1rem;
    font-size: 1.3rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
