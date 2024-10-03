<script setup lang="ts">
import MainHeader from './components/MainHeader.vue'
import NavigationBar from './components/NavigationBar.vue'
import SettingsPage from './components/SettingsPage.vue'
</script>

<template>
  <NavigationBar />
  <div class="main-page">
    <MainHeader>Setting</MainHeader>

    <section class="chosen-page">
      <!-- here should be RouterView -->
      <SettingsPage />
    </section>
  </div>
</template>

<style lang="scss">
#app {
  display: flex;
}
.main-page {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.chosen-page {
  width: 100%;
  height: 100%;
  background-color: #f5f7fa;
  padding: 30px 40px;
}

@media only screen and (max-width: 420px) {
  .chosen-page {
    padding: 25px;
  }
}
</style>
