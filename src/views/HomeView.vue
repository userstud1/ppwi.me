<script setup lang="ts"></script>

<template>
  <section class="hero-section">
    <div class="container">
      <div class="hero-content">
        <span class="badge">
          <i class="material-icons">flare</i> Welcome to WebDev
        </span>
        <h1>We create beautiful digital experiences</h1>
        <p class="subtitle">
          A minimalist approach to design and development. We focus on what
          matters most, delivering clean, functional solutions that stand the test of
          time.
        </p>
        <div class="button-group">
          <RouterLink to="/services" class="btn btn-primary">
            Explore Services
            <i class="material-icons">arrow_forward</i>
          </RouterLink>
          <RouterLink to="/contact" class="btn btn-secondary">Get in Touch</RouterLink>
        </div>
      </div>
      <div class="hero-stats">
        <div class="stat-card">
          <div class="stat-icon-wrapper" style="--icon-bg: #e6f0ff; --icon-color: #2979ff;">
            <i class="material-icons">star</i>
          </div>
          <div class="stat-text">
            <h3>100+ Projects</h3>
            <p>Successfully Delivered</p>
          </div>
        </div>
        <div class="stat-card">
          <div class="stat-icon-wrapper" style="--icon-bg: #e8e6ff; --icon-color: #5856d6;">
            <i class="material-icons">thumb_up</i>
          </div>
          <div class="stat-text">
            <h3>98% Satisfaction</h3>
            <p>Client Rating</p>
          </div>
        </div>
        <div class="stat-card">
          <div class="stat-icon-wrapper" style="--icon-bg: #ffe6f1; --icon-color: #ff2d78;">
            <i class="material-icons">group</i>
          </div>
          <div class="stat-text">
            <h3>50+ Clients</h3>
            <p>Worldwide Trust</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="features-section section-padding">
    <div class="container">
      <div class="features-grid">
        <div class="feature-card">
          <div class="feature-icon-wrapper" style="--icon-bg: #e8e6ff; --icon-color: #5856d6;">
            <i class="material-icons">adjust</i>
          </div>
          <span class="number">01</span>
          <h3>Simplicity</h3>
          <p>We believe in the power of simplicity. Every element serves a purpose.</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon-wrapper" style="--icon-bg: #e8e6ff; --icon-color: #5856d6;">
            <i class="material-icons">star</i>
          </div>
          <span class="number">02</span>
          <h3>Quality</h3>
          <p>Attention to detail in every pixel, every interaction, every line of code.</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon-wrapper" style="--icon-bg: #ffe6f1; --icon-color: #ff2d78;">
            <i class="material-icons">group</i>
          </div>
          <span class="number">03</span>
          <h3>Clarity</h3>
          <p>Clear communication and transparent processes from start to finish.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="about-section section-padding">
    <div class="container">
      <div class="about-content">
        <h2>Built for modern teams</h2>
        <p>
          We understand the challenges of building digital products in today's fast-paced world.
          Our approach combines strategic thinking with beautiful execution to deliver results that matter.
        </p>
        <ul class="about-list">
          <li class="about-list-item">
            <div class="about-list-icon">
              <div class="pulsating-circle"></div>
            </div>
            <div class="about-list-text">
              <h4>User-Centered Design</h4>
              <p>Every decision is made with your users in mind</p>
            </div>
          </li>
          <li class="about-list-item">
            <div class="about-list-icon">
              <div class="pulsating-circle"></div>
            </div>
            <div class="about-list-text">
              <h4>Scalable Solutions</h4>
              <p>Built to grow with your business</p>
            </div>
          </li>
        </ul>
      </div>
      <div class="about-image-wrapper">
        <img src="/assets/images/working team.webp" alt="Our Working Team" />
      </div>
    </div>
  </section>
</template>

<style scoped></style>
