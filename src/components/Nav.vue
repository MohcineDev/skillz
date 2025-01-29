<script>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav>
    <div class="container">

      <RouterLink to="/">Logo</RouterLink>
      <div class="link">

        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/about">Courses</RouterLink>
        <RouterLink to="/about">Contact</RouterLink>
        <RouterLink to="/profile">p</RouterLink>

      </div>
      <div class="auth">
        <RouterLink to="/login">login</RouterLink>
        <RouterLink to="/register">register</RouterLink>

      </div>
    </div>
  </nav>
</template>

<style scoped>
nav {
  box-shadow: 0 2px 2px #aaaaaa8a;
  padding: 5px 0;

}
.router-link-active{
  box-shadow:  0 3px 3px #aaaaaa83;
}
.container {
  max-width: var(--max-width);
  margin: 0 auto;
  padding: 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

a {
  color: var(--dark);
  margin: 0 10px;
  font-weight: 600;
}

.auth a {
  background: var(--blue-dark);
  color: #eee;
  border-radius: 20px;
  padding: 10px 20px;

}
</style>