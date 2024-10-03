<script setup lang="ts">
import EditPhoto from './icons/EditPhoto.vue'
</script>

<template>
  <div class="settings-page">
    <nav class="settings-navigation">
      <button class="settings-nav-button active">Edit Profile</button>
      <button class="settings-nav-button">Preferences</button>
      <button class="settings-nav-button">Security</button>
    </nav>

    <section class="edit-profile-block">
      <div class="edit-photo">
        <img src="/women-hd.png" alt="" />
        <button>
          <EditPhoto />
        </button>
      </div>
      <div class="edit-personal-info">
        <div class="personal-block">
          <div class="one-input">
            <h5>Your Name</h5>
            <input type="text" placeholder="Charlene Reed" />
          </div>
          <div class="one-input">
            <h5>User Name</h5>
            <input type="text" placeholder="Charlene Reed" />
          </div>
        </div>
        <div class="personal-block">
          <div class="one-input">
            <h5>Email</h5>
            <input type="email" placeholder="charlenereed@gmail.com" />
          </div>
          <div class="one-input">
            <h5>Password</h5>
            <input type="password" placeholder="**********" />
          </div>
        </div>
        <div class="personal-block">
          <div class="one-input">
            <h5>Date of Birth</h5>
            <input type="text" placeholder="25 January 1990" />
          </div>
          <div class="one-input">
            <h5>Present Address</h5>
            <input type="text" placeholder="San Jose, California, USA" />
          </div>
        </div>
        <div class="personal-block">
          <div class="one-input">
            <h5>Permanent Address</h5>
            <input type="text" placeholder="San Jose, California, USA" />
          </div>
          <div class="one-input">
            <h5>City</h5>
            <input type="text" placeholder="San Jose" />
          </div>
        </div>
        <div class="personal-block">
          <div class="one-input">
            <h5>Postal Code</h5>
            <input type="text" placeholder="45962" />
          </div>
          <div class="one-input">
            <h5>Country</h5>
            <input type="text" placeholder="USA" />
          </div>
        </div>

        <div class="save-button">
          <button>Save</button>
        </div>
      </div>
    </section>
  </div>
</template>
