<script setup lang="ts"></script>

<template>
  <section class="services-section section-padding">
    <div class="container">
      <div class="section-header">
        <span class="header-pretitle">What We Do</span>
        <h2 class="header-title">Our Services</h2>
        <p class="header-subtitle">
          We specialize in creating exceptional websites for businesses of all sizes. From design to deployment and beyond, we're here for you every step of the way.
        </p>
      </div>

      <div class="service-cards-grid">
        <div class="service-card">
          <div class="service-icon-wrapper" style="--icon-bg: #e6f0ff; --icon-color: #2979ff;">
            <i class="material-icons">draw</i>
          </div>
          <h3 class="service-title">Web Design</h3>
          <p class="service-description">
            Beautiful, user-friendly website designs that capture your brand essence and engage your audience.
          </p>
          <ul class="service-features">
            <li><i class="material-icons">check</i>UI/UX Design</li>
            <li><i class="material-icons">check</i>Responsive Layouts</li>
            <li><i class="material-icons">check</i>Brand Integration</li>
            <li><i class="material-icons">check</i>Prototyping</li>
          </ul>
          <a href="#" class="service-learn-more">
            Learn more <i class="material-icons">arrow_forward</i>
          </a>
        </div>

        <div class="service-card">
          <div class="service-icon-wrapper" style="--icon-bg: #e8e6ff; --icon-color: #5856d6;">
            <i class="material-icons">lightbulb</i>
          </div>
          <h3 class="service-title">Consulting</h3>
          <p class="service-description">
            Expert guidance to help you make informed decisions about your web presence and digital strategy.
          </p>
          <ul class="service-features">
            <li><i class="material-icons">check</i>Technical Consulting</li>
            <li><i class="material-icons">check</i>Strategy Planning</li>
            <li><i class="material-icons">check</i>Best Practices</li>
            <li><i class="material-icons">check</i>Performance Audit</li>
          </ul>
          <a href="#" class="service-learn-more">
            Learn more <i class="material-icons">arrow_forward</i>
          </a>
        </div>

        <div class="service-card">
          <div class="service-icon-wrapper" style="--icon-bg: #ffe6f1; --icon-color: #ff2d78;">
            <i class="material-icons">headset_mic</i>
          </div>
          <h3 class="service-title">Support</h3>
          <p class="service-description">
            Ongoing support and maintenance to keep your website running smoothly and up-to-date.
          </p>
          <ul class="service-features">
            <li><i class="material-icons">check</i>Regular Updates</li>
            <li><i class="material-icons">check</i>Bug Fixes</li>
            <li><i class="material-icons">check</i>Security Monitoring</li>
            <li><i class="material-icons">check</i>24/7 Support</li>
          </ul>
          <a href="#" class="service-learn-more">
            Learn more <i class="material-icons">arrow_forward</i>
          </a>
        </div>
      </div>
    </div>
  </section>

  <section class="process-section section-padding">
    <div class="container">
      <div class="section-header">
        <h2 class="header-title">How We Work</h2>
        <p class="header-subtitle">
          Our streamlined process ensures your website project is delivered on time with exceptional quality.
        </p>
      </div>

      <div class="process-timeline">
        <div class="process-step">
          <div class="process-step-number" style="--step-bg: #2979ff;"><span>1</span></div>
          <h3 class="process-step-title">Consultation</h3>
          <p class="process-step-description">Understanding your vision and business goals</p>
        </div>
        <div class="process-step">
          <div class="process-step-number" style="--step-bg: #5856d6;"><span>2</span></div>
          <h3 class="process-step-title">Design</h3>
          <p class="process-step-description">Creating beautiful mockups and prototypes</p>
        </div>
        <div class="process-step">
          <div class="process-step-number" style="--step-bg: #c62f8f;"><span>3</span></div>
          <h3 class="process-step-title">Development</h3>
          <p class="process-step-description">Building your website with modern tech</p>
        </div>
        <div class="process-step">
          <div class="process-step-number" style="--step-bg: #ff2d78;"><span>4</span></div>
          <h3 class="process-step-title">Launch</h3>
          <p class="process-step-description">Deploying your site to the world</p>
        </div>
        <div class="process-step">
          <div class="process-step-number" style="--step-bg: #ff3b30;"><span>5</span></div>
          <h3 class="process-step-title">Support</h3>
          <p class="process-step-description">Ongoing maintenance and updates</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
