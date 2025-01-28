<script>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav>

    <RouterLink to="/">Logo</RouterLink>
    <div class="link">

        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/about">Courses</RouterLink>
        <RouterLink to="/about">Contact</RouterLink>
    </div>
    <div class="auth">
        <RouterLink to="/login">login</RouterLink>
        <RouterLink to="/register">register</RouterLink>

    </div>
  </nav>
</template>

<style scoped>

nav{
    max-width: 1300px;
    margin: 0 auto;
    padding: 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
margin-top: 10px;
}
a{
    color: #222;
    margin: 0 10px;
    font-weight: 600;
}
.auth a{
background: var(--blue);
color:#eee;
border-radius: 20px;
padding: 10px 20px;

}
</style>