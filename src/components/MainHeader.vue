<script setup lang="ts">
import SettingsIcon from './icons/SettingsIcon.vue'
import NotificationsIcon from './icons/NotificationsIcon.vue'
import HamburgerMenu from './icons/HamburgerMenu.vue'
</script>

<template>
  <header class="main-header">
    <div class="upper-section">
      <button class="hamburger-menu">
        <HamburgerMenu />
      </button>

      <h3 class="current-page-name">
        <slot></slot>
      </h3>
      <div class="header-right-side">
        <div class="header-search-buttons">
          <input type="text" placeholder="Search for something" />

          <button class="header-icon">
            <SettingsIcon />
          </button>
          <button class="header-icon">
            <NotificationsIcon />
          </button>
        </div>
        <button class="header-avatar">
          <img src="/women.png" alt="" />
        </button>
      </div>
    </div>
    <div class="lower-section">
      <div class="header-search-buttons">
        <input type="text" placeholder="Search for something" />
      </div>
    </div>
  </header>
</template>
