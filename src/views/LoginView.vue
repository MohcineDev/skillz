<script setup>
import footerCmp from "../components/footerCmp.vue";
import NavBar from "../components/Nav.vue";
</script>
<template>
  <NavBar />
  <section>

    <div class="login-container">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
        class="arrows">
        <path stroke-linecap="round" stroke-linejoin="round"
          d="M3.75 3.75v4.5m0-4.5h4.5m-4.5 0L9 9M3.75 20.25v-4.5m0 4.5h4.5m-4.5 0L9 15M20.25 3.75h-4.5m4.5 0v4.5m0-4.5L15 9m5.25 11.25h-4.5m4.5 0v-4.5m0 4.5L15 15" />
      </svg>

      <div class="bg">
        <div class="img"></div>
      </div>
      <div class="login-card">
        <h2>Welcome!</h2>
        <form @submit.prevent="handleLogin">
          <div class="input-group">
            <label for="email">Email</label>
            <input type="email" id="email" v-model="email" autocomplete="off" placeholder="Enter your email" required />
          </div>
          <div class="input-group">
            <label for="password">Password</label>
            <input type="password" id="password" v-model="password"  placeholder="Enter your password" required />
          </div>
          <button type="submit" class="login-btn">Login</button>
          <p class="signup-link">
            Don't have an account? <a href="#">Sign Up</a>
          </p>
        </form>
      </div>

    </div>
  </section>
  <footerCmp />
</template>
<style scoped>
section {
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  display: flex;
}

.bg {
  padding: 2rem 0;
}

.img {
  width: 100%;
  height: 100%;
  background: url('../assets/undraw_barista_wwfa.svg') no-repeat center center/ contain;
}

input {
  box-sizing: border-box;
}

.login-container {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.21);
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  max-width: 1000px;
  min-width: 800px;
  position: relative;
  color: #eeeeee73;
}

.arrows {
  position: absolute;
  width: 129px;
  height: 140px;
  z-index: -1;
  top: -60px;
  left: -60px;
  transform: rotate(17deg);
}

.login-card {
  background-color: var(--blue-light);

  color: #fff;
  padding: 4rem 20px;

}

.login-card h2 {
  margin-bottom: 20px;
  font-size: 2rem;
}

.input-group {
  margin-bottom: 15px;
}

.input-group label {
  font-size: 14px;
  display: block;
  margin-bottom: 5px;
}

.input-group input {
  width: 100%;
  padding: 10px;
  font-size: 16px;
  border: 1px solid #ccc;
  border-radius: 5px;
  outline: none;
}

.input-group input:focus {
  border-color: #3b82f6;
}

.login-btn {
  width: 100%;
  padding: 10px;
  background-color: #2d3873;
  color: white;
  border: none;
  border-radius: 5px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.login-btn:hover {
  background-color: #2563eb;
}

.signup-link {
  text-align: center;
  margin-top: 10px;
}

.signup-link a {
  color: #2d3873;
  text-decoration: none;
}

.signup-link a:hover {
  text-decoration: underline;
}
</style>