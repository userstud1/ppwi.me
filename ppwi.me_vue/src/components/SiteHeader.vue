<script setup lang="ts">
import { RouterLink } from 'vue-router'
import { ref } from 'vue'

const mobileOpen = ref(false)
const toggleMobile = () => {
  mobileOpen.value = !mobileOpen.value
}
const closeMobile = () => { mobileOpen.value = false }
</script>

<template>
  <header class="navbar">
    <div class="container">
      <RouterLink to="/" class="logo">
        <div class="logo-icon"></div>
        <span>WebDev</span>
      </RouterLink>
      <button class="mobile-toggle" @click="toggleMobile" :aria-expanded="mobileOpen" aria-controls="main-nav">
        <span class="material-icons">menu</span>
      </button>
      <nav>
        <ul id="main-nav" :class="['nav-links', { open: mobileOpen }]">
          <li>
            <RouterLink to="/" v-slot="{ navigate, href, isActive }">
              <a :href="href" @click.prevent="() => { navigate(); closeMobile() }" :class="{ active: isActive }" :aria-current="isActive ? 'page' : undefined">
                <i class="material-icons">home</i>
                Home
              </a>
            </RouterLink>
          </li>
          <li>
            <RouterLink to="/services" v-slot="{ navigate, href, isActive }">
              <a :href="href" @click.prevent="() => { navigate(); closeMobile() }" :class="{ active: isActive }" :aria-current="isActive ? 'page' : undefined">
                <i class="material-icons">work</i>
                Services
              </a>
            </RouterLink>
          </li>
          <li>
            <RouterLink to="/about" v-slot="{ navigate, href, isActive }">
              <a :href="href" @click.prevent="() => { navigate(); closeMobile() }" :class="{ active: isActive }" :aria-current="isActive ? 'page' : undefined">
                <i class="material-icons">info</i>
                About
              </a>
            </RouterLink>
          </li>
          <li>
            <RouterLink to="/contact" v-slot="{ navigate, href, isActive }">
              <a :href="href" @click.prevent="() => { navigate(); closeMobile() }" :class="{ active: isActive }" :aria-current="isActive ? 'page' : undefined">
                <i class="material-icons">mail</i>
                Contact
              </a>
            </RouterLink>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style scoped>
/***** header-specific overrides can go here if needed *****/
</style>

<style scoped>
/* Mobile toggle button */
.mobile-toggle {
  display: none;
  background: transparent;
  border: none;
  font-size: 1.5rem;
  cursor: pointer;
}

/* Show toggle on small screens */
@media (max-width: 768px) {
  /* Align hamburger on the same row as logo, right side */
  .navbar .container { display: flex; align-items: center; }
  .mobile-toggle {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: .5rem;
    margin-left: auto; /* push to the far right in the flex row */
    width: 40px;
    height: 40px;
  }
  .nav-links { display: none; }
  .nav-links.open {
    display: flex !important;
    flex-direction: column;
    gap: 1rem;
    position: absolute;
    left: 0;
    right: 0;
    top: 72px;
    background: white;
    padding: 1rem 2rem;
    box-shadow: 0 10px 30px rgba(0,0,0,0.06);
  }
  .nav-links.open li a { display: flex; align-items: center; gap: .5rem; }
}
</style>
