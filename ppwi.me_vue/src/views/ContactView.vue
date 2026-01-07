<script setup lang="ts">
import { ref } from 'vue'

const formData = ref({
  firstName: '',
  lastName: '',
  email: '',
  phone: '',
  company: '',
  website: '',
  service: '',
  budget: '',
  timeline: '',
  details: '',
})

const handleSubmit = (e: Event) => {
  e.preventDefault()
  console.log('Form submitted:', formData.value)
  alert('Thank you for your inquiry! We will get back to you within 24 hours.')
}
</script>

<template>
  <section class="contact-hero section-padding">
    <div class="container contact-grid">
      <div class="contact-intro">
        <span class="header-pretitle">Start Your Project</span>
        <h1 class="header-title">Get in Touch</h1>
        <p class="header-subtitle">
          Ready to bring your website vision to life? Fill out the form below and we'll get back to you
          within 24 hours.
        </p>
        <img src="/assets/images/company team image.jpg" alt="Our Team" style="width: 100%; border-radius: 16px; margin-top: 2rem; box-shadow: 0 10px 30px rgba(0,0,0,0.1); flex-grow: 1; object-fit: cover;">
      </div>

      <div class="contact-card contact-info-column">
        <h3>Contact Information</h3>
        <p class="contact-text">Prefer email or a quick call? Reach us using the details below.</p>

        <div class="contact-info-items">
          <div class="contact-info-item" style="--icon-bg:#e6f0ff;--icon-color:#2979ff;">
            <div class="contact-info-icon">
              <i class="material-icons">email</i>
            </div>
            <div>
              <h4>Email</h4>
              <p>hello@minimal.com</p>
            </div>
          </div>

          <div class="contact-info-item" style="--icon-bg:#e8e6ff;--icon-color:#5856d6;">
            <div class="contact-info-icon">
              <i class="material-icons">phone</i>
            </div>
            <div>
              <h4>Phone</h4>
              <p>+1 (234) 567-890</p>
            </div>
          </div>

          <div class="contact-info-item" style="--icon-bg:#ffe6f1;--icon-color:#ff2d78;">
            <div class="contact-info-icon">
              <i class="material-icons">location_on</i>
            </div>
            <div>
              <h4>Location</h4>
              <p>123 Design Street<br>San Francisco, CA 94102</p>
            </div>
          </div>

          <div class="contact-info-item" style="--icon-bg:#fff3e0;--icon-color:#ff9800;">
            <div class="contact-info-icon">
              <i class="material-icons">schedule</i>
            </div>
            <div>
              <h4>Office Hours</h4>
              <p>Mon - Fri: 9:00 AM - 6:00 PM<br>Sat - Sun: Closed</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="section-padding">
    <div class="container contact-layout">
      <div class="contact-form-card">
        <h2 class="contact-form-title">Project Inquiry Form</h2>
        <form class="contact-form" @submit="handleSubmit">
          <div class="form-row">
            <div class="form-group">
              <label for="firstName">First Name *</label>
              <input v-model="formData.firstName" type="text" id="firstName" placeholder="John" required />
            </div>
            <div class="form-group">
              <label for="lastName">Last Name *</label>
              <input v-model="formData.lastName" type="text" id="lastName" placeholder="Doe" required />
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label for="email">Email *</label>
              <input v-model="formData.email" type="email" id="email" placeholder="john@company.com" required />
            </div>
            <div class="form-group">
              <label for="phone">Phone Number</label>
              <input v-model="formData.phone" type="tel" id="phone" placeholder="+1 (234) 567-890" />
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label for="company">Company Name</label>
              <input v-model="formData.company" type="text" id="company" placeholder="Your Company Inc." />
            </div>
            <div class="form-group">
              <label for="website">Current Website (if any)</label>
              <input v-model="formData.website" type="url" id="website" placeholder="https://yourwebsite.com" />
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label for="service">Service Interested In *</label>
              <select v-model="formData.service" id="service" required>
                <option value="" disabled selected>Select a service</option>
                <option>Web Design</option>
                <option>Development</option>
                <option>Consulting</option>
                <option>Support & Maintenance</option>
              </select>
            </div>
            <div class="form-group">
              <label for="budget">Project Budget</label>
              <select v-model="formData.budget" id="budget">
                <option value="" disabled selected>Select budget range</option>
                <option>$1,000 - $3,000</option>
                <option>$3,000 - $7,000</option>
                <option>$7,000 - $15,000</option>
                <option>$15,000+</option>
              </select>
            </div>
          </div>

          <div class="form-row">
            <div class="form-group full">
              <label for="timeline">Expected Timeline</label>
              <select v-model="formData.timeline" id="timeline">
                <option value="" disabled selected>When do you need this completed?</option>
                <option>1-2 Months</option>
                <option>3-4 Months</option>
                <option>5+ Months</option>
                <option>Flexible</option>
              </select>
            </div>
          </div>

          <div class="form-row">
            <div class="form-group full">
              <label for="details">Project Details *</label>
              <textarea v-model="formData.details" id="details" rows="5" placeholder="Tell us about your project, goals, and any specific requirements..." required></textarea>
            </div>
          </div>

          <button type="submit" class="btn btn-primary contact-submit-btn">
            <i class="material-icons">send</i>
            Submit Inquiry
          </button>
        </form>
      </div>

      <aside class="contact-sidebar">
        <div class="contact-sidebar-card" style="--icon-bg:#e6f0ff;--icon-color:#2979ff;">
          <div class="contact-sidebar-icon">
            <i class="material-icons">email</i>
          </div>
          <div class="contact-sidebar-text">
            <h4>Email</h4>
            <p>hello@minimal.com</p>
          </div>
        </div>

        <div class="contact-sidebar-card" style="--icon-bg:#e8e6ff;--icon-color:#5856d6;">
          <div class="contact-sidebar-icon">
            <i class="material-icons">phone</i>
          </div>
          <div class="contact-sidebar-text">
            <h4>Phone</h4>
            <p>+1 (234) 567-890</p>
          </div>
        </div>

        <div class="contact-sidebar-card" style="--icon-bg:#ffe6f1;--icon-color:#ff2d78;">
          <div class="contact-sidebar-icon">
            <i class="material-icons">location_on</i>
          </div>
          <div class="contact-sidebar-text">
            <h4>Location</h4>
            <p>123 Design Street<br>San Francisco, CA 94102</p>
          </div>
        </div>

        <div class="contact-sidebar-card" style="--icon-bg:#fff3e0;--icon-color:#ff9800;">
          <div class="contact-sidebar-icon">
            <i class="material-icons">schedule</i>
          </div>
          <div class="contact-sidebar-text">
            <h4>Office Hours</h4>
            <p>Monday - Friday: 9:00 AM - 6:00 PM<br>Saturday - Sunday: Closed</p>
          </div>
        </div>
      </aside>
    </div>
  </section>
</template>

<style scoped></style>
