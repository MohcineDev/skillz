<script setup>
import { RouterLink, RouterView } from "vue-router";
function toggleNav() {
  const linksContainer = document.querySelector(".links-container");
  linksContainer.classList.toggle("slide-nav");
}
</script>

<template>
  <nav>
    <RouterLink to="/">Logo</RouterLink>
    <div class="links-container">
      <div class="links">
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/about">Courses</RouterLink>
        <RouterLink to="/about">Contact</RouterLink>
      </div>
      <div class="auth">
        <RouterLink to="/login">login</RouterLink>
        <RouterLink to="/register">register</RouterLink>
      </div>
    </div>
    <div class="toggle-nav" @click="toggleNav">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        fill="currentColor"
      >
        <path
          fill-rule="evenodd"
          d="M3 6.75A.75.75 0 0 1 3.75 6h16.5a.75.75 0 0 1 0 1.5H3.75A.75.75 0 0 1 3 6.75ZM3 12a.75.75 0 0 1 .75-.75h16.5a.75.75 0 0 1 0 1.5H3.75A.75.75 0 0 1 3 12Zm0 5.25a.75.75 0 0 1 .75-.75h16.5a.75.75 0 0 1 0 1.5H3.75a.75.75 0 0 1-.75-.75Z"
          clip-rule="evenodd"
        />
      </svg>
    </div>
  </nav>
</template>

<style scoped>
nav {
  max-width: 1300px;
  margin: 0 auto;
  padding: 1rem 10px;
  display: flex;
  justify-content: space-between;
}
.toggle-nav {
  display: none;
  cursor: pointer;
}
.toggle-nav svg {
  pointer-events: none;
}
.links-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.nav-toggle {
  display: none;
}
a {
  color: #222;
  margin: 0 10px;
  font-weight: 600;
}
.auth a {
  background: var(--blue);
  color: #eee;
  border-radius: 20px;
  padding: 10px 20px;
}
@media screen and (max-width: 600px) {
  nav {
    justify-content: space-between;
    padding: 1rem;
  }
  .toggle-nav {
    display: block;
  }
  .links-container {
    position: absolute;
    flex-direction: column;
    background: var(--vt-c-white-soft);
    height: 100vh;
    width: 100%;
    top: 62px;
    left: -100%;
    justify-content: flex-start;
    transition: left 0.3s;
  }
  .links,
  .auth {
    display: flex;
    flex-direction: column;
  }
  .links-container a {
    padding: 1rem 0;
    margin: 1rem;
  }

  .slide-nav {
    left: 0;
  }
}
</style>