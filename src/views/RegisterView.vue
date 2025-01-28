<script setup>
import footerCmp from "../components/footerCmp.vue";
import NavBar from "../components/Nav.vue";
</script>

<template>
  <NavBar />
  <section>
    <div class="register-container">
      <div class="register-card">
        <h2>Register</h2>
        <form @submit.prevent="handleRegister">
          <div class="input-group">
            <label for="email">Email</label>
            <input
              type="email"
              id="email"
              v-model="email"
              placeholder="Enter your email"
              required
            />
          </div>
          <div class="input-group">
            <label for="password">Password</label>
            <input
              type="password"
              id="password"
              v-model="password"
              placeholder="Enter your password"
              required
            />
          </div>
          <div class="input-group">
            <label for="confirm-password">Confirm Password</label>
            <input
              type="password"
              id="confirm-password"
              v-model="confirmPassword"
              placeholder="Confirm your password"
              required
            />
          </div>
          <button type="submit" class="register-btn">Register</button>
          <p class="login-link">
            Already have an account? <a href="#">Login</a>
          </p>
        </form>
      </div>
    </div>
  </section>
  <footerCmp />
</template>

<style scoped>
section {
  display: flex;
  height: 100vh;
  align-items: center;
  justify-content: center;
}
input {
  box-sizing: border-box;
}

.register-container {
  width: 100%;
  max-width: 400px;
  padding: 20px;
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.register-card h2 {
  text-align: center;
  margin-bottom: 20px;
  color: #333;
}

.input-group {
  margin-bottom: 15px;
}

.input-group label {
  font-size: 14px;
  color: #555;
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

.register-btn {
  width: 100%;
  padding: 10px;
  background-color: #3b82f6;
  color: white;
  border: none;
  border-radius: 5px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.register-btn:hover {
  background-color: #2563eb;
}

.login-link {
  text-align: center;
  margin-top: 10px;
}

.login-link a {
  color: #3b82f6;
  text-decoration: none;
}

.login-link a:hover {
  text-decoration: underline;
}
</style>
