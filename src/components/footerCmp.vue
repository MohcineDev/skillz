<template>
  <footer class="footer">
    <div class="container">
      <div class="wrapper">
        <a href="#" class="link">About Us</a>
        <a href="#" class="link">Services</a>
        <a href="#" class="link">Contact</a>
      </div>
      <div class="wrapper">
        <a href="#" class="link">Privacy Policy</a>
        <a href="#" class="link">Terms of Use</a>
        <a href="#" class="link">FAQ</a>
      </div>
      <div class="wrapper">
        <a href="#" class="link">Careers</a>
        <a href="#" class="link">Blog</a>
        <a href="#" class="link">Support</a>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; {{ currentYear }} Your Company. All Rights Reserved.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent',
  data() {
    return {
      currentYear: new Date().getFullYear()
    }
  }
}
</script>

<style scoped>
.footer {
  background-color: var(--blue-dark); /* Dark background */
  color: #ffffff;
  padding: 20px 0;
}
.container {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  max-width: 1200px;
  padding: 20px;
  margin: 0 auto;
}
.wrapper {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.link {
  color: #ffffff;
  text-decoration: none;
  font-size: 14px;
}
.link:hover {
  text-decoration: underline;
}
.footer-bottom {
  text-align: center;
  margin-top: 20px;
  font-size: 12px;
  color: #cccccc;
}
</style>
