<script setup lang="ts"></script>

<template>
  <footer class="site-footer">
    <div class="container">
      <div class="footer-top">
        <div class="footer-brand">
          <a href="#" class="logo">
            <div class="logo-icon"></div>
            <span>WebDev</span>
          </a>
          <p class="footer-tagline">Creating beautiful digital experiences</p>
        </div>
        <div class="footer-links">
          <div class="footer-link-group">
            <h4>Quick Links</h4>
            <ul>
              <li><RouterLink to="/">Home</RouterLink></li>
              <li><RouterLink to="/services">Services</RouterLink></li>
              <li><RouterLink to="/about">About</RouterLink></li>
              <li><RouterLink to="/contact">Contact</RouterLink></li>
            </ul>
          </div>
          <div class="footer-link-group">
            <h4>Legal</h4>
            <ul>
              <li><a href="#">Privacy</a></li>
              <li><a href="#">Terms</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer-bottom">
        <p>© 2025 WebDev. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<style scoped></style>
